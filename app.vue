<script setup>
const darkMode = ref(true)
</script>

<template>
  <div :class="{ 'dark': darkMode }">
    <div class="bg-white dark:bg-dim-900">
      <div class="min-h-full">
        <div class="grid grid-cols-12 mx-auto sm:px-6 lg:max-w-7xl lg:px-8 lg:gap-5">
          <!-- left -->
          <div class="md:block xs:col-span-1 xl:col-span-2">
            <div class="stickey top-0"></div>
            <SidebarLeft />
          </div>
          <!-- main -->
          <main class="col-span-12 md:col-span-8 xl:col-span-6">
            <h1>Main</h1>
          </main>

          <!-- right -->
          <div class="hidden col-span-12 md:block xl:col-span-4 md:col-span-3">
            <div class="sticky top-0">
              <SidebarRight />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

