<template>
  <div class="bg-white">
    <header class="py-8 px-4 md:px-16">
      <div class="container mx-auto flex justify-between items-center">
        <img src="../../img/LendCash_Logo-removebg-preview.png" class="w-20" alt="logo" />
      </div>
    </header>
  </div>

  <div class="max-w-screen-xl mx-auto px-4 md:px-8">
    <div class="items-start justify-between md:flex">
      <div class="max-w-lg">
        <h3 class="text-gray-800 text-xl font-bold sm:text-2xl">LIBRARIES</h3>
      </div>
    </div>

    <!-- Table for Employees and Customers with action buttons -->
    <div class="mt-12 relative h-max overflow-auto">
      <table class="w-full table-auto text-sm text-left">
        <thead class="text-gray-600 font-medium border-b">
          <tr>
            <th class="py-3 pr-6">Categories</th>
            <th class="py-3 pr-6">View</th>
            <th class="py-3 pr-6">Update</th>
            <th class="py-3 pr-6">Delete</th>
          </tr>
        </thead>
        <tbody class="text-gray-600 divide-y">
          <!-- Employees Row -->
          <tr>
            <td class="pr-6 py-4 whitespace-nowrap">Employees</td>
            <td class="pr-6 py-4 whitespace-nowrap">
              <button @click="viewEmployees" class="py-1.5 px-3 bg-gray-200 hover:bg-gray-300 rounded"><a href="EmployeeView">View</a></button>
            </td>
            <td class="pr-6 py-4 whitespace-nowrap">
              <button @click="updateEmployees" class="py-1.5 px-3 bg-blue-200 hover:bg-blue-300 rounded"><a href="EmployeeUpdate">Update</a></button>
            </td>
            <td class="pr-6 py-4 whitespace-nowrap">
              <button @click="deleteEmployees" class="py-1.5 px-3 bg-red-200 hover:bg-red-300 rounded">Delete</button>
            </td>
          </tr>

          <!-- Customers Row -->
          <tr>
            <td class="pr-6 py-4 whitespace-nowrap">Customers</td>
            <td class="pr-6 py-4 whitespace-nowrap">
              <button @click="viewCustomers" class="py-1.5 px-3 bg-gray-200 hover:bg-gray-300 rounded"><a href="CustomerView">View</a></button>
            </td>
            <td class="pr-6 py-4 whitespace-nowrap">
              <button @click="updateCustomers" class="py-1.5 px-3 bg-blue-200 hover:bg-blue-300 rounded"><a href="CustomerUpdate">Update</a></button>
            </td>
            <td class="pr-6 py-4 whitespace-nowrap">
              <button @click="deleteCustomers" class="py-1.5 px-3 bg-red-200 hover:bg-red-300 rounded">Delete</button>
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    viewEmployees() {
      console.log("Viewing Employees");
    },
    updateEmployees() {
      console.log("Updating Employees");
    },
    deleteEmployees() {
      console.log("Deleting Employees");
    },
    viewCustomers() {
      console.log("Viewing Customers");
    },
    updateCustomers() {
      console.log("Updating Customers");
    },
    deleteCustomers() {
      console.log("Deleting Customers");
    }
  }
};
</script>
