<template>
  <div>
    <section class="relative lg:pt-48 lg:pb-64">
      <div class="container flex flex-col-reverse flex-wrap items-center px-2 mx-auto lg:px-0 lg:flex-row">
        <div class="w-full px-4 md:w-8/12 lg:w-6/12 xl:w-6/12">
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
              >Get Started</a>
            </div>
          </div>
        </div>

        <div class="right-0 top-auto w-full lg:absolute md:w-8/12 lg:w-6/12 xl:w-6/12">
          <img
            svg-inline
            class="block w-auto h-auto text-gray-900 fill-current focus:outline-none"
            src="@/assets/svg/home_banner.svg"
          />
        </div>
      </div>
    </section>

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
          <div class="w-full mr-auto -mt-32 md:w-6/12">
            <div class="relative flex flex-wrap justify-center">
              <div class="w-full px-4 my-4 lg:w-6/12">

                <div class="p-8 text-center bg-blue-500 rounded-lg shadow-lg">
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
                    HyperDbg designed to be hidden, it uses different processor feature, virtualizing memory management unit so most of the anti-debugging tricks won't work on HyperDbg.
                  </p>
                </div>

                <div class="p-8 mt-8 text-center bg-green-500 rounded-lg shadow-lg">
                  <div class="inline-flex items-center justify-center w-16 h-16 p-3 bg-white rounded-full shadow-lg">
                    <img
                      svg-inline
                      class="inline-block w-6 h-6 text-gray-600 fill-current focus:outline-none"
                      src="@/assets/svg/bug.svg"
                    />
                  </div>

                  <h6 class="mt-4 text-lg font-semibold text-white">It's a debugger</h6>

                  <p class="mt-2 text-base text-white opacity-75">
                    It's a debugger, even it's not normal debugger, tens of innovative implementations and features make HyperDbg a unique debugger.
                  </p>
                </div>
              </div>

              <div class="w-full px-4 my-4 lg:w-6/12 lg:mt-16">
                <div class="p-8 text-center bg-orange-500 rounded-lg shadow-lg">
                  <div class="inline-flex items-center justify-center w-16 h-16 p-3 bg-white rounded-full shadow-lg">
                    <img
                      svg-inline
                      class="inline-block w-6 h-6 -mt-1 -mr-1 text-gray-600 fill-current focus:outline-none"
                      src="@/assets/svg/puzzle.svg"
                    />
                  </div>

                  <h6 class="mt-4 text-lg font-semibold text-white">It's for reverse engineering</h6>

                  <p class="mt-2 text-base text-white opacity-75">
                    HyperDbg is not a classic debugger, means that we are not limited to just break to the debugger to get a command like Windbg.
                  </p>
                </div>

                <div class="p-8 mt-8 text-center bg-red-600 rounded-lg shadow-lg">
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
                    HyperDbg is based on innovative methods, soon we have more magical commands specially new commands with assist of Intel VT-x and for the future versions, we'll add Intel PT to our debugger.
                  </p>
                </div>
              </div>
            </div>
          </div>

          <div class="w-full px-12 pt-16 ml-auto mr-auto lg:pt-0 md:w-4/12 md:px-4">
            <div class="inline-flex items-center justify-center w-16 h-16 p-3 mb-6 text-center text-gray-600 bg-white rounded-full shadow-lg">
              <i class="text-xl fas fa-drafting-compass">
              </i>
            </div>

            <h3 class="mb-2 text-3xl font-semibold leading-normal">Magic features!</h3>

            <p class="mt-4 mb-4 text-lg font-light leading-relaxed text-gray-700">
              HyperDbg comes with features like hidden hooks, which is as fast as old inline hooks, but also stealth. It mimics hardware debug registers for (read & write) to a specific location, but this time entirely invisible for both Windows kernel and the programs, and of course without any limitation in size or count!
            </p>

            <a
              href="#"
              class="font-bold text-gray-800 hover:text-gray-600"
            >
              Read More ...
            </a>
          </div>
        </div>
      </div>
    </section>

    <section class="relative py-20">
      <div
        class="absolute top-0 left-0 right-0 bottom-auto w-full -mt-20 overflow-hidden pointer-events-none"
        style="height:80px;transform:translateZ(0)"
      ><svg
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
                >Geting Started</a>

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

    <section class="relative block bg-gray-800">
      <div class="container px-4 py-32 mx-auto ">
        <div class="flex flex-wrap justify-center text-center">
          <div class="w-full px-4 lg:w-6/12">
            <h2 class="text-4xl font-semibold text-white">Overview</h2>

            <p class="mt-4 mb-4 text-lg leading-relaxed text-gray-500">
              HyperDbg is extended based on the following assumptions.
            </p>
          </div>
        </div>

        <div class="flex flex-wrap justify-center mt-32">
          <div class="w-full px-4 mb-12 text-left lg:w-4/12">
            <img
              svg-inline
              class="inline-block w-12 h-12 text-gray-600 fill-current focus:outline-none"
              src="@/assets/svg/feature_3.svg"
            />

            <h6 class="mt-5 text-xl font-semibold text-white">Active Development</h6>
            <p class="mt-2 mb-4 text-gray-500">
              HyperDbg is globaly under active development, many people contribute in its design.
            </p>
          </div>

          <div class="w-full px-4 mb-12 text-left lg:w-4/12">
            <img
              svg-inline
              class="inline-block w-12 h-12 text-gray-600 fill-current focus:outline-none"
              src="@/assets/svg/feature_1.svg"
            />

            <h5 class="mt-5 text-xl font-semibold text-white">
              Rely on Academic Papers
            </h5>

            <p class="mt-2 mb-4 text-gray-500">
              We extend HyperDbg's new features based on academic papers.
            </p>
          </div>

          <div class="w-full px-4 mb-12 text-left lg:w-4/12">
            <img
              svg-inline
              class="inline-block w-12 h-12 text-gray-600 fill-current focus:outline-none"
              src="@/assets/svg/feature_2.svg"
            />

            <h5 class="mt-5 text-xl font-semibold text-white">Custom Scripts</h5>
            <p class="mt-2 mb-4 text-gray-500">
              You can create custom Python scripts and use all HyperDbg features automatically in a way you want.
            </p>
          </div>

          <div class="w-full px-4 mb-12 text-left lg:w-4/12">
            <img
              svg-inline
              class="inline-block w-12 h-12 text-gray-600 fill-current focus:outline-none"
              src="@/assets/svg/feature_6.svg"
            />

            <h5 class="mt-5 text-xl font-semibold text-white">Integration with Static Analysis Tools</h5>
            <p class="mt-2 mb-4 text-gray-500">
              One of the goals of HyperDbg is to make an easy integration with static analysis tools like IDA, Ghidra and other tools.
            </p>
          </div>

          <div class="w-full px-4 mb-12 text-left lg:w-4/12">
            <img
              svg-inline
              class="inline-block w-12 h-12 text-gray-600 fill-current focus:outline-none"
              src="@/assets/svg/feature_5.svg"
            />

            <h5 class="mt-5 text-xl font-semibold text-white">Heavily Hardware-dependant</h5>
            <p class="mt-2 mb-4 text-gray-500">
              HyperDbg extensively uses hardware technologies to ease the reverse-engineering.
            </p>
          </div>

          <div class="w-full px-4 mb-12 text-left lg:w-4/12">
            <img
              svg-inline
              class="inline-block w-12 h-12 text-gray-600 fill-current focus:outline-none"
              src="@/assets/svg/feature_4.svg"
            />

            <h5 class="mt-5 text-xl font-semibold text-white">Have a New Idea?</h5>
            <p class="mt-2 mb-4 text-gray-500">
              Open an issue and describe how to implement it or you can submit a pull request with you feature.
            </p>
          </div>
        </div>

      </div>
    </section>

    <section class="relative py-20">

      <div class="container px-4 mx-auto lg:my-64">
        <div class="flex flex-wrap items-center">
          <div class="right-0 top-auto w-full lg:absolute md:w-8/12 lg:w-6/12 xl:w-6/12">
            <img
              svg-inline
              class="block w-auto h-auto text-gray-900 fill-current focus:outline-none"
              src="@/assets/svg/question.svg"
            />
          </div>

          <div class="w-full px-4 mr-auto md:w-6/12">
            <div class="md:pl-12">

              <h3 class="text-3xl font-semibold text-gray-800">
                FAQs
              </h3>

              <p class="mt-3 text-lg leading-relaxed text-gray-600">
                Here's a fast guide of how to compile and run HyperDbg on your system, also there are some interesting examples of how you can use HyperDbg in your reverse-engineering journey.
              </p>

            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>

export default {
  name: 'Home'
}
</script>
