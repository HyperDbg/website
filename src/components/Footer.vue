<template>
  <footer class="relative pt-8 pb-6 bg-gray-300">
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
          class="text-gray-300 fill-current"
          points="2560 0 2560 100 0 100"
        ></polygon>
      </svg>
    </div>

    <div class="container px-4 mx-auto">
      <div class="flex flex-wrap">
        <div class="w-full px-4 md:w-6/12">
          <h4 class="text-3xl font-semibold text-gray-900">What's HyperDbg?</h4>

          <h5 class="mt-2 mb-3 text-sm text-gray-700">
            HyperDbg is an open-source, user-mode, and kernel-mode debugger that relies on hardware features to debug the Windows Kernel and Applications. It's mainly designed based on Intel Virtualization Technology (VT-x).
          </h5>

          <div class="flex mt-6">
            <a
              class="mr-4"
              href="https://twitter.com/HyperDbg"
              target="_blank"
            >
              <img
                svg-inline
                class="block w-6 h-6 text-gray-600 fill-current focus:outline-none hover:text-red-500"
                src="@/assets/svg/twitter.svg"
              />
            </a>

            <a
              class="mr-3"
              href="https://github.com/HyperDbg"
              target="_blank"
            >
              <img
                svg-inline
                class="block w-6 h-6 text-gray-600 fill-current focus:outline-none hover:text-red-500"
                src="@/assets/svg/github.svg"
              />
            </a>
          </div>
          <p class="mt-6 text-sm font-semibold text-gray-600">It's under GPLv3
            <a
              href="https://github.com/HyperDbg/HyperDbg/blob/master/LICENSE"
              targe="_blank"
              class="text-gray-700"
            >LICENSE</a>.
          </p>
        </div>

        <div class="w-full px-4 md:w-6/12">
          <div class="flex flex-wrap mb-6 items-top">
            <div class="w-full pt-6 ml-auto md:w-6/12 xl:w-4/12 md:pt-0 md:px-4">

              <span class="block mb-2 text-sm font-semibold text-gray-600 uppercase">Resources</span>

              <ul class="list-unstyled">
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://github.com/HyperDbg/HyperDbg/releases"
                    target="_blank"
                  >Download</a>
                </li>

                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://docs.hyperdbg.com/"
                    target="_blank"
                  >Documentation</a>
                </li>

                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://github.com/HyperDbg/HyperDbg"
                    target="_blank"
                  >Source</a>
                </li>

                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://github.com/HyperDbg/HyperDbg/issues"
                    target="_blank"
                  >Issues</a>
                </li>
              </ul>
            </div>

            <div class="w-full pt-6 ml-auto md:w-6/12 xl:w-4/12 md:pt-0 md:px-4">

              <span class="block mb-2 text-sm font-semibold text-gray-600 uppercase">Useful Links</span>

              <ul class="list-unstyled">
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://rayanfam.com/contact/"
                    target="_blank"
                  >Contact Us</a>
                </li>

                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://rayanfam.com/tutorials/"
                    target="_blank"
                  >Tutorials</a>
                </li>

                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://rayanfam.com/"
                    target="_blank"
                  >Blog</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <hr class="my-6 border-gray-400">
      <div class="flex flex-wrap items-center justify-center md:justify-between">
        <div class="w-full px-4 mx-auto text-center md:w-4/12">
          <div class="py-1 text-sm font-semibold text-gray-600 whitespace-no-wrap">
            Copyright &copy; 2020 All rights reserved.
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style>
</style>
