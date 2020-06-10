<template>
  <section class="relative py-20">
    <div
      class="absolute top-0 left-0 right-0 bottom-auto w-full -mt-20 overflow-hidden pointer-events-none"
      style="height:80px;transform:translateZ(0)"
    >
      <svg
        class="absolute bottom-0 overflow-hidden"
        xmlns="http://www.w3.org/2000/svg"
        preserveAspectRatio="none"
        version="1.1"
        viewBox="0 0 2560 100"
        x="0"
        y="0"
      >
        <polygon
          class="text-white fill-current"
          points="2560 0 2560 100 0 100"
        ></polygon>
      </svg>
    </div>

    <div class="container px-4 mx-auto lg:my-64">
      <div class="flex flex-wrap items-center">
        <div class="left-0 top-auto w-full lg:absolute md:w-8/12 lg:w-6/12">
          <img
            svg-inline
            class="block w-auto h-auto text-gray-900 fill-current focus:outline-none"
            src="@/assets/svg/get_started.svg"
          />
        </div>

        <div class="w-full px-4 ml-auto md:w-6/12">
          <div class="md:pl-12">

            <h3 class="text-3xl font-semibold text-gray-800">How to start with HyperDbg?</h3>

            <p class="mt-3 text-lg leading-relaxed text-gray-600">
              Here's a fast guide of how to compile and run HyperDbg on your system, also there are some interesting examples of how you can use HyperDbg in your reverse-engineering journey.
            </p>

            <div class="mt-12">
              <a
                href="https://docs.hyperdbg.com/getting-started"
                class="inline-block px-6 py-4 text-sm font-bold text-white bg-red-500 rounded shadow outline-none hover:bg-red-600 github-star focus:outline-none active:bg-gray-700 hover:shadow-lg"
                target="_blank"
              >Getting Started</a>

              <a
                href="https://docs.hyperdbg.com/using-hyperdbg/"
                class="px-6 py-4 text-sm font-bold text-white bg-yellow-500 rounded shadow outline-none lg:ml-1 hover:bg-yellow-600 github-star focus:outline-none active:bg-gray-700 hover:shadow-lg"
                target="_blank"
              >HyperDbg Examples</a>
            </div>

          </div>
        </div>
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
