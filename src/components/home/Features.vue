<template>
  <section class="relative pb-40 mt-40 bg-gray-200">
    <div
      class="absolute top-0 left-0 right-0 bottom-auto w-full -mt-20"
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
          class="text-gray-200 fill-current"
          points="2560 0 2560 100 0 100"
        ></polygon>
      </svg>
    </div>

    <div class="container mx-auto">
      <div class="flex flex-wrap items-center">
        <div class="w-full mx-auto -mt-32 xl:ml-0 md:w-8/12 xl:w-6/12">
          <div class="relative flex flex-wrap justify-center">
            <div class="w-full px-4 my-4 lg:w-6/12">

              <div class="p-8 text-center bg-blue-500 rounded-lg shadow-lg cursor-default hover:bg-blue-600">
                <div class="inline-flex items-center justify-center w-16 h-16 p-3 bg-white rounded-full shadow-lg">
                  <img
                    svg-inline
                    class="inline-block w-6 h-6 text-gray-600 fill-current focus:outline-none"
                    src="@/assets/svg/ghost.svg"
                  />
                </div>

                <h6 class="mt-4 text-lg font-semibold text-white">
                  It's hidden
                </h6>

                <p class="mt-2 text-base text-white opacity-75">
                  HyperDbg is designed to be hidden, it uses different processor features, virtualizing memory management unit so most of the anti-debugging tricks won't work on HyperDbg.                </p>
              </div>

              <div class="p-8 mt-8 text-center bg-green-500 rounded-lg shadow-lg cursor-default hover:bg-green-600">
                <div class="inline-flex items-center justify-center w-16 h-16 p-3 bg-white rounded-full shadow-lg">
                  <img
                    svg-inline
                    class="inline-block w-6 h-6 text-gray-600 fill-current focus:outline-none"
                    src="@/assets/svg/bug.svg"
                  />
                </div>

                <h6 class="mt-4 text-lg font-semibold text-white">It's a debugger</h6>

                <p class="mt-2 text-base text-white opacity-75">
                  It's a debugger, even it's not a normal debugger, tens of innovative implementations and features make HyperDbg a unique debugger.                </p>
              </div>
            </div>

            <div class="w-full px-4 my-4 lg:w-6/12 lg:mt-16">
              <div class="p-8 text-center bg-orange-500 rounded-lg shadow-lg cursor-default hover:bg-orange-600">
                <div class="inline-flex items-center justify-center w-16 h-16 p-3 bg-white rounded-full shadow-lg">
                  <img
                    svg-inline
                    class="inline-block w-6 h-6 -mt-1 -mr-1 text-gray-600 fill-current focus:outline-none"
                    src="@/assets/svg/puzzle.svg"
                  />
                </div>

                <h6 class="mt-4 text-lg font-semibold text-white">It's for reverse engineering</h6>

                <p class="mt-2 text-base text-white opacity-75">
                  HyperDbg is not a classic debugger, which means that we are not limited to just break to the debugger to get a command like Windbg.                </p>
              </div>

              <div class="p-8 mt-8 text-center bg-red-600 rounded-lg shadow-lg cursor-default hover:bg-red-700">
                <div class="inline-flex items-center justify-center w-16 h-16 p-3 bg-white rounded-full shadow-lg">
                  <img
                    svg-inline
                    class="inline-block w-6 h-6 text-gray-600 fill-current focus:outline-none"
                    src="@/assets/svg/magic.svg"
                  />
                </div>

                <h6 class="mt-4 text-lg font-semibold text-white">
                  Magical Commands
                </h6>

                <p class="mt-2 text-base text-white opacity-75">
                  HyperDbg is based on innovative methods, soon we have more magical commands especially new commands with the assist of Intel VT-x and for the future versions, we'll add Intel PT to our debugger.                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="w-full px-8 pt-16 ml-auto mr-auto md:w-8/12 xl:w-4/12">
          <div class="inline-flex items-center justify-center w-16 h-16 p-3 mb-6 text-center text-gray-600 bg-white rounded-full shadow-lg">
            <img
              svg-inline
              class="inline-block w-6 h-6 text-gray-600 fill-current focus:outline-none"
              src="@/assets/svg/features.svg"
            />
          </div>

          <h3 class="mb-2 text-3xl font-semibold leading-normal">Innovative Features!</h3>

          <p class="mt-4 mb-8 text-lg font-light leading-relaxed text-gray-700">
            HyperDbg comes with features like hidden hooks, which is as fast as old inline hooks, but also stealth. It mimics hardware debug registers for (read & write) to a specific location, but this time entirely invisible for both Windows kernel and the programs, and of course without any limitation in size or count!
          </p>

          <a
            href="https://docs.hyperdbg.com/design/features"
            class="font-bold text-gray-800 hover:text-red-600"
          >
            Read More ...
          </a>
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
