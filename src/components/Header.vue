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
                href="https://docs.hyperdbg.com/"
              >Documentation</a>
            </li>

            <li class="flex items-center">
              <a
                class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                href="https://doxygen.hyperdbg.com/"
              >Doxygen</a>
            </li>

            <li class="flex items-center">
              <div class="relative">
                <button
                  class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2 focus:outline-none"
                  @click="showTutorials = ! showTutorials"
                >Hypervisor Tutorial
                  <svg
                    class="w-5 h-5 ml-2 -mr-1"
                    viewBox="0 0 20 20"
                    fill="currentColor"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </button>

                <div
                  class="left-0 z-50 w-56 origin-top-right rounded-md lg:mt-2 lg:shadow-lg lg:absolute lg:ml-3"
                  v-show="showTutorials"
                >
                  <div
                    class="bg-white rounded-md lg:border lg:shadow-sm"
                    role="menu"
                    aria-orientation="vertical"
                    aria-labelledby="options-menu"
                  >
                    <div class="py-1">
                      <a
                        :key="index"
                        v-for="(item, index) in tutorials"
                        :href="item.link"
                        class="block px-4 py-2 text-sm leading-5 text-gray-700 hover:bg-gray-100 hover:text-gray-900 focus:outline-none focus:bg-gray-100 focus:text-gray-900"
                        role="menuitem"
                        v-text="item.title"
                      ></a>
                    </div>
                  </div>
                </div>

              </div>
            </li>

            <li class="flex items-center">
              <a
                class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                href="https://rayanfam.com/"
              >Blog</a>
            </li>
          </ul>

          <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between list-none lg:justify-end lg:ml-auto">
            <ul class="flex list-none">
              <li class="flex items-center">
                <a
                  class="flex items-center py-4 pr-3 text-gray-800 lg:px-3 lg:py-2"
                  href="https://twitter.com/HyperDbg"
                >
                  <img
                    svg-inline
                    class="inline-block w-6 h-6 text-gray-700 fill-current hover:text-red-500"
                    src="@/assets/svg/twitter.svg"
                  />
                </a>
              </li>

              <li class="flex items-center">
                <a
                  class="flex items-center py-4 text-gray-800 lg:px-3 lg:py-2"
                  href="https://github.com/HyperDbg"
                >
                  <img
                    svg-inline
                    class="inline-block w-6 h-6 text-gray-700 fill-current hover:text-red-500"
                    src="@/assets/svg/github.svg"
                  />
                </a>
              </li>
            </ul>

            <ul class="flex list-none sm:my-4 lg:ml-3">
              <li class="flex items-center">
                <a
                  href="/download"
                  class="flex items-center px-4 py-2 text-sm font-bold text-white uppercase bg-red-500 rounded shadow outline-none active:bg-gray-100 hover:shadow-md focus:outline-none hover:bg-red-600 hover:shadow-lg"
                >
                  <img
                    svg-inline
                    src="@/assets/svg/download.svg"
                    class="inline-block w-3 h-3 mr-2 text-white fill-current"
                  />
                  <span>Download</span>
                </a>
              </li>

              <li class="flex items-center">
                <a
                  href="#"
                  class="flex items-center px-4 py-2 ml-3 text-sm font-bold text-white uppercase bg-indigo-500 rounded shadow outline-none active:bg-gray-100 hover:shadow-md focus:outline-none hover:bg-indigo-600 hover:shadow-lg"
                >
                  <img
                    svg-inline
                    src="@/assets/svg/quote.svg"
                    class="inline-block w-3 h-3 mr-2 fill-current"
                  />
                  <span>Cite Paper</span>
                </a>
              </li>
            </ul>
          </div>
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
      showMenu: false,

      showTutorials: false,
      tutorials: [
        { title: 'Part 1', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-1/' },
        { title: 'Part 2', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-2/' },
        { title: 'Part 3', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-3/' },
        { title: 'Part 4', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-4/' },
        { title: 'Part 5', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-5/' },
        { title: 'Part 6', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-6/' },
        { title: 'Part 7', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-7/' },
        { title: 'Part 8', link: 'https://rayanfam.com/topics/hypervisor-from-scratch-part-8/' }
      ]
    }
  },

  methods: {
    toggleNavbar: function () {
      this.showMenu = !this.showMenu
    }
  }
}
</script>
