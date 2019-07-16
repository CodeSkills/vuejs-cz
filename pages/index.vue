<template>
  <div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
    <h2 class="text-4xl inline-flex">Česká a Slovenská komunita <img class="mx-3"
           src="~/assets/logo.png"
           style="width: 48px" /> Vue.js</h2>
    <div class="flex flex-wrap">
      <div class="w-full md:w-3/5 mx-auto"
           style="padding-top: 40px">
        <h3 class="py-3 text-2xl">Předchozí meetupy</h3>
        <div class="flex mb-4 border text-left"
             style="opacity: 0.7">
          <img class="w-2/5 flex-auto"
               data-src="https://secure.meetupstatic.com/photos/event/4/e/8/d/highres_482180109.jpeg"
               alt="Thumbnail [200x250]"
               src="https://secure.meetupstatic.com/photos/event/4/e/8/d/highres_482180109.jpeg"
               data-holder-rendered="true">
          <div class="w-3/5 p-4">
            <strong class="inline-block mb-2 text-green-600">Brno Vue.js Meetup #1</strong>
            <h3 class="mb-0">
              <a class="text-grey-800 text-3xl"
                 href="https://www.meetup.com/vuejs-cz-sk/events/262254837/"
                 target="_blank">Úvod do světa Vue.js</a>
            </h3>
            <div class="mb-1 text-gray-600">16. Července 18:30 - 20:00</div>
            <p class="card-text mb-auto text-left"
               style="height: 59px">Po úspěchu v Praze, startuje nyní naše raketa i z Brna. A všichni smělí astronauti jsou srdečně zváni.</p>
            <a href="https://docs.google.com/presentation/d/1qdCnLoPRYF4QSvbpf8cuTjU0HyuxD1ufnEa9hosC_So/edit?usp=sharing"
               class="px-2"> &#128190; Úvod do Vue.js</a>
            <a href="https://docs.google.com/presentation/d/1WEUVu7cRXrrBCXJ6R1HEXucRjN6xe6wae9WGrXBOvmY/edit?usp=sharing"
               class="px-2"> &#128190; Ekosystém Vue.js</a>
            <a href="https://docs.google.com/presentation/d/1ovYhJdg2m9UNMWO8YJkDBHdzDdcC0IHfnUld0whHcNE/edit?usp=sharing"
               class="px-2"> &#128190; Live Demo</a><br><br>

            <div class=""><a href="https://www.meetup.com/vuejs-cz-sk/events/262254837/"
                 target="_blank"
                 class="text-green-600 mt-4">Zobrazit meetup</a></div>
          </div>
        </div>
        <div class="flex mb-4 border text-left"
             style="opacity: 0.7">
          <img class="w-2/5 flex-auto"
               data-src="https://secure.meetupstatic.com/photos/event/7/c/b/b/highres_481411931.jpeg"
               alt="Thumbnail [200x250]"
               src="https://secure.meetupstatic.com/photos/event/7/c/b/b/highres_481411931.jpeg"
               data-holder-rendered="true"
               style="width: 450px; height: 260px;">
          <div class="w-3/5 p-4">
            <strong class="d-inline-block mb-2 text-green-600">Prague Vue.js Meetup #7</strong>
            <h3 class="mb-0">
              <a class="text-grey-800 text-3xl"
                 href="https://www.meetup.com/vuejsprague/events/259864138/"
                 target="_blank">State of Vue.js 2019</a>
            </h3>
            <div class="mb-1 text-gray-600">23. Května 18:30 - 20:30</div>
            <p class="card-text mb-auto text-left"
               style="height: 59px">Připravujeme pro vás další Vue.js Meetup. <br>Tentokrát na téma "State of Vue.js 2019".</p>
            <a href="https://docs.google.com/presentation/d/13AF5808CNo2rB2egyLHNiLFJh3MF7ScQtUIGIzLSZgg/edit?usp=sharing"
               class="px-2"> &#128190; Stav Vue.js 2019</a>
            <a href="https://www.dropbox.com/s/i9wa8ha9cuzld3b/Vue.js%203.0.key?dl=0"
               class="px-2"> &#128190; Vue.js 3.0</a>
            <a href="https://drive.google.com/file/d/1DyvmrH7poDavgcIim_xtOLpOhEkmBwMc/view?usp=sharing"
               class="px-2"> &#128190; Vue.js Devtools 5.0</a><br><br>
            <a href="https://www.meetup.com/vuejsprague/events/259864138/"
               target="_blank"
               class="text-green-600 mt-2">Zobrazit meetup</a>
          </div>
        </div>
      </div>
      <div class="col-md-2"
           style="display:none">
        <iframe src="https://discordapp.com/widget?id=561595492719525948&theme=dark"
                width="350"
                height="500"
                allowtransparency="true"
                frameborder="0"></iframe>
      </div>
    </div>
    <!-- Global site tag (gtag.js) - Google Analytics -->

  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
