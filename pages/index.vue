<template>
  <div class="bg-white">
    <header class="py-8 px-4 md:px-16">
      <div class="container mx-auto flex justify-between items-center">
        <img src="../img/LendCash_Logo-removebg-preview.png" class="w-20" alt="logo">
        <!-- <h1 class="text-3xl font-bold text-gray-800">LendCash</h1> -->
        <nav class="hidden md:flex gap-10">
          <a href="libraries/library" class="text-gray-600 hover:text-gray-800 font-bold">Features</a>
          <a href="pricing" class="text-gray-600 hover:text-gray-800 font-bold">Pricing</a>
          <a href="about" class="text-gray-600 hover:text-gray-800 font-bold">About</a>
          <a href="/" class="text-gray-600 hover:text-gray-800 font-bold">Blog</a>
          <a href="contact" class="text-gray-600 hover:text-gray-800 font-bold">Contact</a>
          <!-- <a href="#" class="bg-blue-500 text-white px-4 py-2 rounded-md hover:bg-blue-600">Pro Version</a> -->
        </nav>
        <div class="flex gap-4">
          <a href="login" class="text-black hover:text-gray-800 font-bold">Log in</a>
          <a href="register-form" class="text-black hover:text-green-900 font-bold">Sign Up</a>
          <!-- <button class="bg-blue-500 text-white px-4 py-2 rounded-md hover:bg-blue-600">Sign up</button> -->
        </div>
      </div>
    </header>
    <main class="py-16 px-4 md:px-16">
      <div class="container mx-auto flex flex-col md:flex-row gap-16">
        <div class="md:w-1/2">
          <h2 class="text-5xl font-bold text-gray-800 mb-4">LendCash Microfinance System for ERD Financial Solution </h2>
          <p class="text-lg text-gray-600 mb-8">An Online Microfinance Lending System.</p>
          <div class="flex gap-4">
            <button class="bg-black text-white px-4 py-2 rounded-md hover:bg-green-900">Apply Now</button>
            <!-- <button class="bg-gray-200 text-gray-800 px-4 py-2 rounded-md hover:bg-gray-300">GitHub Repo</button> -->
          </div>
        </div>
        <div class="md:w-1/2 flex justify-center items-center">
          <img src="../img/handsakebg_1sect.jpg" alt="LendCash-Logo" class="w-50 h-50 float-right">
        </div>
      </div>
      <div class="container mx-auto mt-20">
        <h3 class="text-4xl font-bold text-gray-800 mb-4">LendCash Offers</h3>
        <p class="text-lg text-gray-600 mb-8">Creating Opportunities, One Microloan at a Time.</p>
        <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mt-8">
          <div class="bg-gray-100 rounded-md p-4 shadow-md items-center justify-center">
            <img src="../img/grouping.png" alt="Icon 1" class="w-50 h-50">
            <h4 class="text-xl font-bold text-gray-800 mb-2">Group Lending</h4>
            <p class="text-gray-600">Offers small groups of individuals come together to access financial services. In this system, members guarantee each other's loans, fostering a sense of shared responsibility and mutual support.</p>
          </div>
          <div class="bg-gray-100 rounded-md p-4 shadow-md items-center justify-center">
            <img src="../img/no-hidden-fees.png" alt="Icon 1" class="w-50 h-50 items-center">
            <h4 class="text-xl font-bold text-gray-800 mb-2">No Surcharges</h4>
            <p class="text-gray-600">Providing loans and financial services without additional fees beyond the agreed interest rates. This approach ensures that borrowers are not burdened with hidden costs or extra charges, making financial products more transparent and accessible.</p>
          </div>
          <div class="bg-gray-100 rounded-md p-4 shadow-md items-center justify-center">
            <img src="../img/no-collaretal.png" alt="Icon 1" class="w-50 h-50 items-center">
            <h4 class="text-xl font-bold text-gray-800 mb-2">No Collateral</h4>
            <p class="text-gray-600">Providing loans and financial services without requiring borrowers to pledge assets as security. This approach enables individuals, particularly those with limited or no assets, to access credit and other financial services.</p>
          </div>
          <div class="bg-gray-100 rounded-md p-4 shadow-md items-center justify-center">
            <img src="../img/easy-loan-process.png" alt="Icon 1" class="w-50 h-50 items-center">
            <h4 class="text-xl font-bold text-gray-800 mb-2">Easy Loan Process</h4>
            <p class="text-gray-600">Experience a seamless and straightforward loan process designed to make borrowing as easy as possible. Our easy loan process is tailored to reduce the complexity and time typically associated with securing a loan, so you can focus on what matters most.</p>
          </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mt-6">
          <div class="bg-gray-100 rounded-md p-4 shadow-md items-center justify-center">
            <img src="../img/loan-disbursement.png" alt="Icon 1" class="w-50 h-50 items-center">
            <h4 class="text-xl font-bold text-gray-800 mb-2">Quick Cash Disbursement</h4>
            <p class="text-gray-600">When you need access to funds quickly, our quick cash disbursement service is here to meet your needs. We understand that timely financial support is crucial, and we’ve streamlined our process to ensure that you receive your cash swiftly and efficiently.</p>
          </div>
          <div class="bg-gray-100 rounded-md p-4 shadow-md items-center justify-center">
            <img src="../img/hassle-free.png" alt="Icon 1" class="w-50 h-50 items-center">
            <h4 class="text-xl font-bold text-gray-800 mb-2">Hassle Free Requirements</h4>
            <p class="text-gray-600">Aim to simplify the borrowing process, making it more accessible and efficient for borrowers while ensuring that lenders can accurately assess risk and compliance. This approach reduces the complexity and time involved in securing a loan, creating a smoother experience for all parties.</p>
          </div>
        </div>
      </div>
      <section class="py-14">
        <div class="max-w-screen-xl mx-auto px-4 md:px-8">
            <div class="max-w-xl sm:text-center md:mx-auto">
              <div class="pb-6">
                <img src="../img/LendCash_Logo-removebg-preview.png"  class="mx-auto w-20" />
              </div>
                <h3 class="text-gray-800 text-3xl font-semibold sm:text-4xl">
                    See what others saying about us
                </h3>
                <p class="mt-3 text-gray-600">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc et est hendrerit, porta nunc vitae, gravida justo. Nunc fermentum magna lorem, euismod volutpat arcu volutpat et.
                </p>
            </div>
            <div class="mt-12">
                <ul class="grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
                    <li v-for="(item, idx) in testimonials" :key="idx" class="bg-gray-100 p-4 rounded-xl">
                        <figure>
                            <div class="flex items-center gap-x-4">
                                <img :src="item.avatar" class="w-16 h-16 rounded-full" />
                                <div>
                                    <span class="block text-gray-800 font-semibold">{{ item.name }}</span>
                                    <span class="block text-gray-600 text-sm mt-0.5">{{ item.title }}</span>
                                </div>
                            </div>
                            <blockquote>
                                <p class="mt-6 text-gray-700">
                                    {{ item.quote }}
                                </p>
                            </blockquote>
                        </figure>
                    </li>
                </ul>
            </div>
        </div>
      </section>
    </main>
    <footer class="pt-10 bg-gray-800">
    <div class="max-w-screen-xl mx-auto px-4 md:px-8">
      <div class="justify-between items-center gap-12 md:flex">
        <div class="flex-1 max-w-lg">
          <h3 class="text-white text-2xl font-bold">
            Get our beautiful newsletter straight to your inbox.
          </h3>
        </div>
        <div class="flex-1 mt-6 md:mt-0">
          <form @submit.prevent="onSubmit" class="flex items-center gap-x-3 md:justify-end">
            <div class="relative">
              <svg
                class="w-6 h-6 text-gray-400 absolute left-3 inset-y-0 my-auto"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                strokeWidth="{1.5}"
                stroke="currentColor"
              >
                <path
                  strokeLinecap="round"
                  strokeLinejoin="round"
                  d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75"
                />
              </svg>
              <input
                type="email"
                required
                placeholder="Enter your email"
                class="w-full pl-12 pr-3 py-2 text-gray-500 bg-white outline-none border focus:border-indigo-600 shadow-sm rounded-lg"
              />
            </div>
            <button class="block w-auto py-3 px-4 font-medium text-sm text-center text-white bg-indigo-600 hover:bg-indigo-500 active:bg-indigo-700 active:shadow-none rounded-lg shadow">
              Subscribe
            </button>
          </form>
        </div>
      </div>
      <div class="flex-1 mt-16 space-y-6 justify-between sm:flex md:space-y-0">
        <ul v-for="(item, idx) in footerNavs" :key="idx" class="space-y-4 text-gray-300">
          <h4 class="text-gray-200 font-semibold sm:pb-2">{{ item.label }}</h4>
          <li v-for="(el, index) in item.items" :key="index">
            <a :href="el.href" class="duration-150 hover:text-gray-400">{{ el.name }}</a>
          </li>
        </ul>
      </div>
      <div class="mt-10 py-10 border-t border-gray-700 items-center justify-between sm:flex">
        <p class="text-gray-300">© 2024 LendCash. All rights reserved.</p>
        <div class="flex items-center gap-x-6 text-gray-400 mt-6">
          <a href="javascript:void()">
            <svg
              class="w-6 h-6 hover:text-gray-500 duration-150"
              fill="none"
              viewBox="0 0 48 48"
            >
              <g clip-path="url(#a)">
                <path
                  fill="currentColor"
                  d="M48 24C48 10.745 37.255 0 24 0S0 10.745 0 24c0 11.979 8.776 21.908 20.25 23.708v-16.77h-6.094V24h6.094v-5.288c0-6.014 3.583-9.337 9.065-9.337 2.625 0 5.372.469 5.372.469v5.906h-3.026c-2.981 0-3.911 1.85-3.911 3.75V24h6.656l-1.064 6.938H27.75v16.77C39.224 45.908 48 35.978 48 24z"
                />
              </g>
              <defs>
                <clipPath id="a">
                  <path fill="#fff" d="M0 0h48v48H0z" />
                </clipPath>
              </defs>
            </svg>
          </a>
          <a href="javascript:void()">
            <svg
              class="w-6 h-6 hover:text-gray-500 duration-150"
              fill="none"
              viewBox="0 0 48 48"
            >
              <g clip-path="url(#clip0_17_80)">
                <path
                  fill="currentColor"
                  d="M15.1 43.5c18.11 0 28.017-15.006 28.017-28.016 0-.422-.01-.853-.029-1.275A19.998 19.998 0 0048 9.11c-1.795.798-3.7 1.32-5.652 1.546a9.9 9.9 0 004.33-5.445 19.794 19.794 0 01-6.251 2.39 9.86 9.86 0 00-16.788 8.979A27.97 27.97 0 013.346 6.299 9.859 9.859 0 006.393 19.44a9.86 9.86 0 01-4.462-1.228v.122a9.844 9.844 0 007.901 9.656 9.788 9.788 0 01-4.442.169 9.867 9.867 0 009.195 6.843A19.75 19.75 0 010 39.078 27.937 27.937 0 0015.1 43.5z"
                />
              </g>
              <defs>
                <clipPath id="clip0_17_80">
                  <path fill="#fff" d="M0 0h48v48H0z" />
                </clipPath>
              </defs>
            </svg>
          </a>
          <a href="javascript:void()">
            <svg
              class="w-6 h-6 hover:text-gray-500 duration-150"
              fill="none"
              viewBox="0 0 48 48"
            >
              <g fill="currentColor" clip-path="url(#clip0_910_44)">
                <path
                  fill-rule="evenodd"
                  d="M24 1A24.086 24.086 0 008.454 6.693 23.834 23.834 0 00.319 21.044a23.754 23.754 0 003.153 16.172 23.98 23.98 0 0012.938 10.29c1.192.221 1.641-.518 1.641-1.146 0-.628-.024-2.45-.032-4.442-6.676 1.443-8.087-2.817-8.087-2.817-1.089-2.766-2.663-3.493-2.663-3.493-2.178-1.478.163-1.45.163-1.45 2.413.17 3.68 2.461 3.68 2.461 2.138 3.648 5.616 2.593 6.983 1.976.215-1.545.838-2.596 1.526-3.193-5.333-.6-10.937-2.647-10.937-11.791a9.213 9.213 0 012.472-6.406c-.246-.6-1.069-3.026.234-6.322 0 0 2.015-.64 6.602 2.446a22.904 22.904 0 0112.017 0c4.583-3.086 6.594-2.446 6.594-2.446 1.307 3.288.484 5.714.238 6.322a9.194 9.194 0 012.476 6.414c0 9.163-5.615 11.183-10.957 11.772.859.742 1.626 2.193 1.626 4.421 0 3.193-.028 5.762-.028 6.548 0 .636.433 1.38 1.65 1.146a23.98 23.98 0 0012.938-10.291 23.754 23.754 0 003.151-16.175A23.834 23.834 0 0039.56 6.69 24.086 24.086 0 0024.009 1H24z"
                  clip-rule="evenodd"
                />
                <path
                  d="M9.089 35.264c-.052.119-.243.154-.398.071-.155-.083-.27-.237-.214-.36.056-.122.242-.154.397-.07.155.082.274.24.215.359zM10.063 36.343a.4.4 0 01-.493-.11c-.155-.167-.187-.396-.068-.499.12-.102.334-.055.489.11.155.167.19.396.072.499zM11.008 37.714c-.147.103-.397 0-.536-.206a.395.395 0 010-.569c.147-.098.397 0 .537.202.139.202.143.47 0 .573zM12.292 39.042c-.131.146-.397.106-.616-.091-.219-.198-.27-.467-.139-.609.131-.142.397-.102.624.091.226.194.27.466.131.609zM14.092 39.816c-.06.186-.33.269-.6.19-.27-.08-.449-.3-.397-.49.051-.19.326-.277.6-.19.274.087.449.297.397.49zM16.056 39.95c0 .194-.223.36-.509.364-.286.004-.52-.154-.52-.348 0-.193.222-.36.508-.363.286-.004.52.15.52.347zM17.884 39.646c.036.194-.163.395-.45.443-.285.047-.536-.067-.572-.257-.035-.19.171-.395.45-.447.278-.05.536.068.572.261z"
                />
              </g>
              <defs>
                <clipPath id="clip0_910_44">
                  <path fill="#fff" d="M0 0h48v48H0z" />
                </clipPath>
              </defs>
            </svg>
          </a>
          <a href="javascript:void()">
            <svg
              class="w-6 h-6 hover:text-gray-500 duration-150"
              fill="currentColor"
              viewBox="0 0 48 48"
            >
              <g clip-path="url(#clip0_17_63)">
                <path
                  d="M24 4.322c6.413 0 7.172.028 9.694.14 2.343.104 3.61.497 4.453.825 1.116.432 1.922.957 2.756 1.791.844.844 1.36 1.64 1.79 2.756.329.844.723 2.12.826 4.454.112 2.53.14 3.29.14 9.693 0 6.413-.028 7.172-.14 9.694-.103 2.344-.497 3.61-.825 4.453-.431 1.116-.957 1.922-1.79 2.756-.845.844-1.642 1.36-2.757 1.791-.844.328-2.119.722-4.453.825-2.532.112-3.29.14-9.694.14-6.413 0-7.172-.028-9.694-.14-2.343-.103-3.61-.497-4.453-.825-1.115-.431-1.922-.956-2.756-1.79-.844-.844-1.36-1.641-1.79-2.757-.329-.844-.723-2.119-.826-4.453-.112-2.531-.14-3.29-.14-9.694 0-6.412.028-7.172.14-9.694.103-2.343.497-3.609.825-4.453.431-1.115.957-1.921 1.79-2.756.845-.844 1.642-1.36 2.757-1.79.844-.329 2.119-.722 4.453-.825 2.522-.113 3.281-.141 9.694-.141zM24 0c-6.516 0-7.331.028-9.89.14-2.55.113-4.304.526-5.822 1.116-1.585.619-2.926 1.435-4.257 2.775-1.34 1.332-2.156 2.672-2.775 4.247C.666 9.806.253 11.55.141 14.1.028 16.669 0 17.484 0 24s.028 7.331.14 9.89c.113 2.55.526 4.304 1.116 5.822.619 1.585 1.435 2.925 2.775 4.257a11.732 11.732 0 004.247 2.765c1.528.591 3.272 1.003 5.822 1.116 2.56.112 3.375.14 9.89.14 6.516 0 7.332-.028 9.891-.14 2.55-.113 4.303-.525 5.822-1.116a11.732 11.732 0 004.247-2.765 11.732 11.732 0 002.766-4.247c.59-1.528 1.003-3.272 1.115-5.822.113-2.56.14-3.375.14-9.89 0-6.516-.027-7.332-.14-9.891-.112-2.55-.525-4.303-1.115-5.822-.591-1.594-1.407-2.935-2.747-4.266a11.732 11.732 0 00-4.247-2.765C38.194.675 36.45.262 33.9.15 31.331.028 30.516 0 24 0z"
                />
                <path
                  d="M24 11.672c-6.806 0-12.328 5.522-12.328 12.328 0 6.806 5.522 12.328 12.328 12.328 6.806 0 12.328-5.522 12.328-12.328 0-6.806-5.522-12.328-12.328-12.328zm0 20.325a7.998 7.998 0 010-15.994 7.998 7.998 0 010 15.994zM39.694 11.184a2.879 2.879 0 11-2.878-2.878 2.885 2.885 0 012.878 2.878z"
                />
              </g>
              <defs>
                <clipPath id="clip0_17_63">
                  <path d="M0 0h48v48H0z" />
                </clipPath>
              </defs>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </footer>
  </div>
</template>

<script>
export default {
    data() {
        return {
            testimonials: [
                {
                    avatar: "https://scontent.fcgy1-1.fna.fbcdn.net/v/t39.30808-6/359522345_3677315609221786_2310243283905235556_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeH6khA-JSL5k2spkEGbg-Mue4vlWqoJXyp7i-VaqglfKgi3G8P41Rpp3h0tbwawZqZFG6Z8Rir5C1VxE2FaA80D&_nc_ohc=8lMHSC7W4PAQ7kNvgEUCqFO&_nc_ht=scontent.fcgy1-1.fna&oh=00_AYCJ5wuDNsPbMMW3d4gQJfOTYDVojdEUH47uwU2IW4WjpQ&oe=66DD3051",
                    name: "Heinz Kyle Hora",
                    title: "Founder of MGG",
                    quote: "Nice."
                },
                {
                    avatar: "https://scontent.fcgy1-1.fna.fbcdn.net/v/t39.30808-6/448656158_1629887417845685_6398441375725225275_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeGeOFE4asStHUlOZco6oK80qfpuDRI2IeOp-m4NEjYh40Yfk9OO0p0f7HpySF7PqhcbrJBkcX2sr3R9Pn5858cV&_nc_ohc=Kc-Vzrd_MaMQ7kNvgHPtz4b&_nc_ht=scontent.fcgy1-1.fna&oh=00_AYB2rdBHgfFwsYFCQsUO500kJHlACjQT79cJNjy48G8RSg&oe=66DD354A",
                    name: "Stephen Duray",
                    title: "Founder of MGG",
                    quote: "Nice."
                },
                {
                    avatar: "https://scontent.fcgy1-1.fna.fbcdn.net/v/t1.15752-9/457869417_880139523982024_8057426980193137924_n.png?_nc_cat=104&ccb=1-7&_nc_sid=9f807c&_nc_eui2=AeHLQdw0XWAnaNothpVh5ogysuphZSIDa5my6mFlIgNrmSjUcm8ZpKHlFiLj_4_bzV7MJ7G-xEP9lN4RnQwoh_Ip&_nc_ohc=TTESbs8EOu0Q7kNvgHy49e8&_nc_ht=scontent.fcgy1-1.fna&oh=03_Q7cD1QEhuLSmpNsAiFORrI0fSu6jnTsBxH83driAhl4viXPJZg&oe=66FEF935",
                    name: "Venn Lopez",
                    title: "Founder of MGG",
                    quote: "Nice."
                },
            ]
        };
    }
}
</script>

<style>
body {
  font-family: 'Inter', sans-serif;
}

.container {
  max-width: 1200px;
}

</style>