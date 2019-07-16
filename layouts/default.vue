<template>
  <div>
    <nav class="flex items-center justify-between flex-wrap p-6">
      <div class="flex items-center flex-shrink-0 text-white mr-6">
        <img src="~/assets/newlogo.png"
             style="width: 48px"
             class="mr-2" />
        <h5 class="my-0 mr-md-auto font-weight-normal">Vuejs.cz</h5>
      </div>
      <div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto">
        <div class="text-sm lg:flex-grow text-right">
          <a class="block mt-4 lg:inline-block lg:mt-0 px-3"
             href="/">Úvod</a>
          <a class="block mt-4 lg:inline-block lg:mt-0 px-3"
             href="/team">Náš tým</a>
          <a class="block mt-4 lg:inline-block lg:mt-0 "
             href="https://www.meetup.com/vuejsprague/"
             target="_blank">
            <img src="~/assets/meetup.png"
                 style="width: 32px; margin-top: -6px"
                 class="mr-1 float-left" />Meetupy</a>
          <a class="block mt-4 lg:inline-block lg:mt-0 px-3"
             href="https://discord.gg/mDr2z8V"
             target="_blank">
            <img src="~/assets/discord.png"
                 style="width: 32px; margin-top: -6px"
                 class="mr-1 float-left" />Discord</a>
          <a class="block mt-4 lg:inline-block lg:mt-0 px-3"
             style="display: none"
             href="#">
            <img src="~/assets/vimeo.png"
                 style="width: 22px; margin-top: -4px"
                 class="mr-2" />Záznamy</a>
          <a class="block mt-4 lg:inline-block lg:mt-0 px-3"
             style="display: none"
             href="/discuss">Diskuze</a>
        </div>
        <div>
          <a class="btn btn-outline-primary"
             style="display: none"
             href="#">Sign up</a>
        </div>
      </div>
    </nav>

    <nuxt />

    <div class="container mx-auto" style="min-height: 0">
      <footer class="w-full pt-4 md:my-5 md:pt-5 border-t">
        <div class="flex flex-wrap text-left">
          <div class="w-1/4">
            <img class="mb-2"
                 src="~/assets/logo.png"
                 alt=""
                 width="24"
                 height="24">
            <small class="d-block mb-3 text-muted">© {{ (new Date()).getFullYear() }}</small>
          </div>
          <div class="w-1/4">
            <h5 class="text-gray-600">Vue knihovny</h5>
            <ul class="list-unstyled text-small">
              <li>
                <a class="text-muted"
                   href="https://vuejs.org/"
                   target="_blank">Vue.js</a>
              </li>
              <li>
                <a class="text-muted"
                   href="https://router.vuejs.org/"
                   target="_blank">Vue Router</a>
              </li>
              <li>
                <a class="text-muted"
                   href="https://vuex.vuejs.org/"
                   target="_blank">Vuex</a>
              </li>
              <li>
                <a class="text-muted"
                   href="https://ssr.vuejs.org/"
                   target="_blank">Vue SSR</a>
              </li>
            </ul>
          </div>
          <div class="w-1/4">
            <h5 class="text-gray-600">Nástroje</h5>
            <ul class="list-unstyled text-small">
              <li>
                <a class="text-muted"
                   href="https://github.com/vuejs/vue-devtools"
                   target="_blank">Devtools</a>
              </li>
              <li>
                <a class="text-muted"
                   href="https://cli.vuejs.org/"
                   target="_blank">Vue CLI</a>
              </li>
              <li>
                <a class="text-muted"
                   href="https://vue-loader.vuejs.org/"
                   target="_blank">Vue Loader</a>
              </li>
            </ul>
          </div>
          <div class="w-1/4 col-md">
            <h5 class="text-gray-600">Komunita</h5>
            <ul class="list-unstyled text-small">
              <li>
                <a class="text-muted"
                   href="/team">Náš tým</a>
              </li>
              <li>
                <a class="text-muted"
                   href="https://discord.gg/mDr2z8V"
                   target="_blank">Discord</a>
              </li>
              <li>
                <a class="text-muted"
                   href="https://www.meetup.com/vuejsprague/"
                   target="_blank">Meetupy</a>
              </li>
            </ul>
          </div>
        </div>
      </footer>
    </div>

  </div>
</template>