<template>
  <nav>
    <!-- Desktop Menu -->
    <div class="bg-gray-300 flex justify-around">
      <!-- Menu-->
      <div class="flex justify-around flex-grow">
        <!-- Logo-->
        <div class="flex items-center py-4 px-2">
          <a class="hover:hover:bg-opacity-20 hover:bg-gray-50">
            <img
              class="w-14"
              src="/img/logo.png"
            >
          </a>
          <span class="pl-5 text-2xl">Gray Area Knives</span>
        </div>
        <!-- Pages-->
        <ul class="flex flex-row px-1 items-center">
          <li>
            <NuxtLink
              class="hover:bg-opacity-20 hover:bg-gray-50 hover:text-primary-600 px-2"
              to="/"
            >
              Home
            </NuxtLink>
          </li>
          <li>
            <NuxtLink
              class="hover:bg-opacity-20 hover:bg-gray-50 hover:text-primary-600 px-2"
              to="/about"
            >
              About Us
            </NuxtLink>
          </li>
          <li>
            <dropdown-menu
              v-model="show"
              :right="right"
              :hover="hover"
              :interactive="interactive"
            >
              <div class="btn btn-primary dropdown-toggle">
                Social
              </div>
            </dropdown-menu>
          </li>
        </ul>
      </div>
      <!-- Login? Button -->
      <div />
    </div>
    <!-- Mobile Menu -->
    <div />
  </nav>
</template>

<script>
export default {};
</script>

<style></style>
