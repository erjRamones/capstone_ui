<template>
  <div class="bg-white p-4 md:p-8">
    <h2 class="text-gray-800 text-xl font-bold mb-4">Edit Employee</h2>

    <form @submit.prevent="updateEmployee">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <!-- Personality Fields -->
        <div>
          <label for="firstName" class="block text-gray-700">First Name</label>
          <input v-model="personality.first_name" type="text" id="firstName" class="w-full border rounded-lg px-4 py-2" required />
        </div>

        <div>
          <label for="lastName" class="block text-gray-700">Last Name</label>
          <input v-model="personality.family_name" type="text" id="lastName" class="w-full border rounded-lg px-4 py-2" required />
        </div>

        <div>
          <label for="middleName" class="block text-gray-700">Middle Name</label>
          <input v-model="personality.middle_name" type="text" id="middleName" class="w-full border rounded-lg px-4 py-2" required />
        </div>

        <div>
          <label for="email" class="block text-gray-700">Email</label>
          <input v-model="personality.email_address" type="email" id="email" class="w-full border rounded-lg px-4 py-2" required />
        </div>

        <div>
          <label for="telephone" class="block text-gray-700">Telephone#</label>
          <input v-model="personality.telephone_no" type="text" id="telephone" class="w-full border rounded-lg px-4 py-2" />
        </div>

        <div>
          <label for="birthday" class="block text-gray-700">Birthday</label>
          <input v-model="personality.birthday" type="date" id="birthday" class="w-full border rounded-lg px-4 py-2" required />
        </div>

        <div>
          <label for="gender" class="block text-gray-700">Gender</label>
          <select v-model="personality.gender_code" id="gender" class="w-full border rounded-lg px-4 py-2">
            <option value="1">Male</option>
            <option value="2">Female</option>
          </select>
        </div>

        <div>
          <label for="civilStatus" class="block text-gray-700">Civil Status</label>
          <select v-model="personality.civil_status" id="civilStatus" class="w-full border rounded-lg px-4 py-2">
            <option value="0">Select</option>
            <option value="1">Single</option>
            <option value="2">Married</option>
            <option value="3">Divorced</option>
            <option value="4">Widowed</option>
          </select>
        </div>

        <div>
          <label for="houseStreet" class="block text-gray-700">House Street</label>
          <input v-model="personality.house_street" type="text" id="houseStreet" class="w-full border rounded-lg px-4 py-2" />
        </div>

        <div>
          <label for="purokZone" class="block text-gray-700">Purok Zone</label>
          <input v-model="personality.purok_zone" type="text" id="purokZone" class="w-full border rounded-lg px-4 py-2" />
        </div>

        <!-- Employee Fields -->
        <div>
          <label for="sss_no" class="block text-gray-700">SSS No.</label>
          <input v-model="employees.sss_no" type="number" id="sss_no" class="w-full border rounded-lg px-4 py-2" />
        </div>

        <div>
          <label for="phic_no" class="block text-gray-700">PhilHealth No.</label>
          <input v-model="employees.phic_no" type="number" id="phic_no" class="w-full border rounded-lg px-4 py-2" />
        </div>

        <div>
          <label for="tin_no" class="block text-gray-700">TIN No.</label>
          <input v-model="employees.tin_no" type="number" id="tin_no" class="w-full border rounded-lg px-4 py-2" />
        </div>
      </div>

      <div>
          <label for="dateTimeRegistered" class="block text-gray-700">Date Time Registered</label>
          <input v-model="personality.datetime_registered" type="date" id="dateTimeRegistered" class="w-full border rounded-lg px-4 py-2" />
        </div>
        <div>
          <label for="dateTimeHired" class="block text-gray-700">Date Time Hired</label>
          <input v-model="employees.datetime_hired" type="date" id="dateTimeHired" class="w-full border rounded-lg px-4 py-2" />
        </div>
        <div>
          <label for="dateTimeResigned" class="block text-gray-700">Date Time Resigned</label>
          <input v-model="employees.datetime_resigned" type="date" id="dateTimeResigned" class="w-full border rounded-lg px-4 py-2" />
        </div>

      <div class="mt-4">
        <button type="submit" class="px-4 py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-500">
          Update Employee
        </button>
      </div>
    </form>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import { useRoute, useRouter } from 'vue-router';
import { EmployeesService } from '~/models/Employee';
import { apiService } from '~/routes/api/API';

const route = useRoute();
const router = useRouter();

const personality = ref({
  first_name: '',
  family_name: '',
  middle_name: '',
  email_address: '',
  telephone_no: '',
  birthday: new Date().toISOString().split('T')[0], // Set to current date
  gender_code: 0, // Default or set as needed (1 for Male, 2 for Female)
  civil_status: 0, // Default or set as needed
  house_street: '',
  purok_zone: '',
  postal_code: '',
  cellphone_no: '',
  personality_status_code: 0,
  barangay_id: 0,
  city_id: 0,
  country_id: 0,
  province_id: 0,
  // credit_status_id: 0,
  notes: undefined, // Optional
  datetime_registered: new Date().toISOString().split('T')[0],
  name_type_code: 0,
})

const employees = ref({
    sss_no: 0,
    phic_no: 0,        //set
    tin_no: 0,
    datetime_hired: undefined, // Optional
    datetime_resigned: undefined, // Optional
  
});


// Call the fetch function
fetchEmployeeData();

function formatDateTimeToMySQL(date: any) {
  const pad = (num: any) => (num < 10 ? '0' + num : num);
  const year = date.getFullYear();
  const month = pad(date.getMonth() + 1);
  const day = pad(date.getDate());
  const hours = pad(date.getHours());
  const minutes = pad(date.getMinutes());
  const seconds = pad(date.getSeconds());
  
  return `${year}-${month}-${day} ${hours}:${minutes}:${seconds}`; // Return as Y-m-d H:i:s
}

function formatDateToMySQL(date: any) {
  const pad = (num: any) => (num < 10 ? '0' + num : num);
  const year = date.getFullYear();
  const month = pad(date.getMonth() + 1); // Months are zero-based
  const day = pad(date.getDate());
  const hours = pad(date.getHours());
  const minutes = pad(date.getMinutes());
  const seconds = pad(date.getSeconds());
  
  return `${year}-${month}-${day} ${hours}:${minutes}:${seconds}`;
}


// Fetch customer data when the component is mounted
async function fetchEmployeeData() {
  const employeeId = EmployeesService.id;
  debugger;
  // Check if customerId is defined and is a valid number
  if (!employeeId || isNaN(Number(employeeId))) {
    alert('Invalid Employee ID');
    navigateTo('/Libraries/EmployeeView'); // Redirect to the customer list page or show an error
    return;
  } // Assuming you pass the ID in the route
  const response = await apiService.getEmployeeById([],employeeId);
  console.log('Employee ID:', employeeId);
  debugger; // Fetch customer data
  Object.assign(employees.value, response.employees);
  Object.assign(personality.value, response.personality) // Merge response data into customer
}


const updateEmployee = async () => {
  try {
    const employeeID = EmployeesService.id;
    // Check if customerId is defined and is a valid number
    if (!employeeID || isNaN(Number(employeeID))) {
      alert('Invalid Employee ID');
      router.push('/employee'); // Redirect to the customer list page or show an error
      return;
    }
    
    const jsonObject = {
      employee: {
            sss_no: employees.value.sss_no,
            phic_no: employees.value.phic_no,        //set
            tin_no: employees.value.tin_no,
            datetime_hired: employees.value.datetime_hired, // Optional
            datetime_resigned: employees.value.datetime_resigned, 
        },
        personality: {
            datetime_registered: personality.value.datetime_registered,
            family_name: personality.value.family_name, // Get from personality ref
            middle_name: personality.value.middle_name, // Assuming this remains unchanged
            first_name: personality.value.first_name, // Get from personality ref
            birthday: personality.value.birthday, // Get from personality ref
            civil_status: personality.value.civil_status, // Get from personality ref
            gender_code: personality.value.gender_code, // Get from personality ref
            house_street: personality.value.house_street, // Get from personality ref
            purok_zone: personality.value.purok_zone, // Get from personality ref
            postal_code: personality.value.postal_code, // Get from personality ref
            telephone_no: personality.value.telephone_no, // Get from personality ref
            email_address: personality.value.email_address, // Get from personality ref
            cellphone_no: personality.value.cellphone_no, // Get from personality ref
            name_type_code: personality.value.name_type_code, // Assuming this remains unchanged
            personality_status_code: personality.value.personality_status_code, // Get from personality ref
            barangay_id: personality.value.barangay_id, // Get from personality ref
            city_id: personality.value.city_id, // Get from personality ref
            country_id: personality.value.country_id, // Get from personality ref
            province_id: personality.value.province_id, // Get from personality ref
            notes: personality.value.notes, // Get from personality ref, optional
        }
    };

    debugger;
    await apiService.updateEmployee(jsonObject, employeeID);
    alert('Employee updated successfully!');
    navigateTo('/Libraries/EmployeeView'); // Redirect to the customer list page
  } catch (error) {
    alert('Error updating employee: ' + error);
    console.error(error);
  }
};
</script>