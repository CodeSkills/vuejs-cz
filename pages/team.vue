<template>
  <div class="mx-auto px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
    <div class="flex flex-wrap text-center align-center justify-center">
      <h2 class="w-full text-4xl pb-6">Náš tým</h2>
      <div class="container">
        <div class="w-3/4" style="display: table; margin: 0 auto;">
          <div class="flex flex-wrap justify-center">
            <div v-for="(person, i) in people" :key="'person' + i" class="flex lg:w-1/2 items-center px-10 pb-20">
              <div class="w-32 h-32 rounded-full overflow-hidden shadow-inner bg-purple mr-3">
                <img :src="`${person.img}`"
                  :alt="person.name"
                  class="object-cover object-center w-32 h-32 visible group-hover:hidden" />
              </div>
              <div class="text-left">
                <div class="text-2xl text-green-600">{{person.name}}</div>
                <a :href="`mailto:${person.email}`" class="text-gray-600">{{ person.email }}</a>
                <div class="flex mt-1">
                  <a v-if="person.linkedin" :href="person.linkedin" class="mr-1"><img src="~/assets/icons/linkedin.svg" :alt="`${person.name} - LinkedIn`" class="opacity-25"></a>
                  <a v-if="person.twitter" :href="person.twitter" class="mr-1"><img src="~/assets/icons/twitter.svg" :alt="`${person.name} - Twitter`" class="opacity-25"></a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Global site tag (gtag.js) - Google Analytics -->
    <script async
            src="https://www.googletagmanager.com/gtag/js?id=UA-67019611-4"></script>
    <script>
    window.dataLayer = window.dataLayer || [];

    function gtag() {
      dataLayer.push(arguments);
    }
    gtag('js', new Date());
    gtag('config', 'UA-67019611-4');
    </script>

  </div>
</template>

<script>
export default {
  name: 'Team',
  data() {
    return {
      people:[
        {
          name: 'Jiří Žižka, MBA',
          email: "george@vuejs.cz",
          img: require('~/assets/team/george.jpg'),
          linkedin: "https://www.linkedin.com/in/jiri-zizka/",
          twitter: "https://twitter.com/GeorgeZizka"
        },
        {
          name: 'Kirill Bunin',
          email: "kirill@vuejs.cz",
          img: require('~/assets/team/kirill.jpeg'),
          linkedin: "https://www.linkedin.com/in/kirillbunin/",
          twitter: "https://twitter.com/kirill_bunin"
        },
        {
          name: 'Libor Vaněk',
          email: "lv@liborvanek.cz",
          img: require('~/assets/team/libor.jpg'),
          linkedin: "https://www.linkedin.com/in/liborvanekcz/",
          twitter: "https://twitter.com/liborvanek"
        },
        {
          name: 'Ondřej Janošík',
          // email: "ondrej@vuejs.cz",
          img: require('~/assets/team/ondrej.jpeg'),
          // linkedin: "https",
          // twitter: "https"
        },
        {
          name: 'Kamil Tomšík',
          // email: "kamil@vuejs.cz",
          img: require('~/assets/team/kamil.jpeg'),
          // linkedin: "https",
          // twitter: "https"
        }
      ]
    }
  }  
}
</script>
