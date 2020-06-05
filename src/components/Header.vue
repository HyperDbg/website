<template>
  <header>
    <nav class="flex flex-wrap items-center justify-between w-full px-2 py-8">
      <div class="container flex flex-wrap items-baseline justify-between px-4 mx-auto">
        <div class="relative flex justify-between w-full lg:w-auto lg:static lg:block lg:justify-start">

          <a
            href="/"
            class="text-2xl"
          >
            HyperDbg Debugger
          </a>

          <button
            class="block py-1 border border-transparent outline-none cursor-pointer lg:hidden focus:outline-none"
            type="button"
            v-on:click="toggleNavbar()"
          >
            <img
              svg-inline
              v-if="!showMenu"
              class="inline-block w-6 h-6 text-gray-900 border-none fill-current focus:outline-none"
              src="@/assets/svg/menu.svg"
            />

            <img
              v-else
              svg-inline
              class="inline-block w-6 h-6 text-gray-900 border-none fill-current focus:outline-none"
              src="@/assets/svg/close.svg"
            />
          </button>
        </div>

        <div
          class="items-center flex-grow lg:flex"
          :class="{'hidden': !showMenu, 'block': showMenu}"
        >
          <ul class="flex flex-col mt-6 list-none lg:ml-16 lg:mt-0 lg:flex-row">
            <li class="flex items-center">
              <a
                class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                href=""
              >Documents</a>
            </li>

            <li class="flex items-center">
              <a
                class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                href=""
              >Doxygen</a>
            </li>

            <li class="flex items-center">
              <a
                class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                href=""
              >Hypervisor Tutorial</a>
            </li>

            <li class="flex items-center">
              <a
                class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                href=""
              >Blog</a>
            </li>
          </ul>

          <ul class="flex items-center justify-between list-none lg:justify-end lg:ml-auto">
            <li class="flex items-center">
              <a
                class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                href=""
              >
                <img
                  svg-inline
                  class="inline-block w-6 h-6 text-gray-900 fill-current"
                  src="@/assets/svg/github.svg"
                />
              </a>
            </li>

            <li class="flex items-center">
              <button class="px-4 py-2 ml-3 text-sm font-bold text-white uppercase bg-red-500 rounded shadow outline-none active:bg-gray-100 hover:shadow-md focus:outline-none">
                Download
              </button>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>

export default {
  components: {
  },

  data () {
    return {
      showMenu: false
    }
  },

  methods: {
    toggleNavbar: function () {
      this.showMenu = !this.showMenu
    }
  }
}
</script>
