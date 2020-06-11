<template>
  <section class="relative pb-32 xl:pt-48 xl:pb-64">
    <div class="container flex flex-col-reverse flex-wrap items-center px-2 mx-auto xl:px-0 xl:flex-row">
      <div class="w-full px-4 sm:mt-12 xl:mt-0 md:w-8/12 xl:w-6/12">
        <div class="pt-32 sm:pt-0">
          <h2 class="text-2xl font-semibold text-gray-700 lg:text-4xl">HyperDbg Debugger</h2>
          <p class="mt-4 text-xl font-semibold leading-relaxed text-gray-600">A debugger designed for analyzing, fuzzing and reversing.</p>

          <p class="mt-4 text-lg leading-relaxed text-gray-600">
            HyperDbg debugger is an open-source, user-mode, and kernel-mode debugger with a focus on using hardware technologies to provide new features to the debuggers’ world.
          </p>

          <div class="mt-16">
            <a
              href="https://docs.hyperdbg.com/getting-started/build-and-install"
              class="px-6 py-4 text-sm font-bold text-white uppercase bg-red-500 rounded shadow outline-none hover:bg-red-600 github-star focus:outline-none active:bg-gray-700 hover:shadow-lg"
              target="_blank"
            >Getting Started</a>
          </div>
        </div>
      </div>

      <div class="right-0 top-auto w-full xl:absolute md:w-8/12 xl:w-6/12">
        <img
          svg-inline
          class="block w-auto h-auto text-gray-900 fill-current focus:outline-none"
          src="@/assets/svg/home_banner.svg"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style>
</style>
