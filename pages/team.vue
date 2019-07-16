<template>
  <div class="mx-auto px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
    <div class="flex flex-wrap text-center align-center justify-center">
      <h2 class="w-full text-4xl pb-6">Náš tým</h2>
      <div v-for="person in people" class="flex w-full justify-center relative mb-4">
        <div  class="flex w-1/4 justify-center border rounded-full p-4 bg-gray-100">
          <div class="w-32 h-32 rounded-full overflow-hidden shadow-inner text-center bg-purple table cursor-pointer">
            <img :src="`${person.img}`"
                 alt="lovely avatar"
                 class="object-cover object-center w-32 h-32 visible group-hover:hidden" />
          </div>
          <div class="w-3/5 px-4 text-center pt-4">
            <div class="text-2xl text-green-600">{{person.name}}</div>
            <div class="text-md text-gray-700">{{person.post}}</div>
            <div class="text-md text-gray-600">{{person.does}}</div>
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
          img: require('~/assets/team/george.jpg'),
          post: 'Hlavní organizátor',
          does: 'Meetupy & školení'  
        },
        {
          name: 'Libor Vaněk',
          img: require('~/assets/team/libor.jpg'),
          post: 'Hlavní organizátor - Praha',
          does: 'Meetupy'  
        },
        {
          name: 'Kirill Bunin',
          img: require('~/assets/team/kirill.jpeg'),
          post: 'Organizátor - Praha',
          does: 'Meetupy'  
        },
        {
          name: 'Ondřej Janošík',
          img: require('~/assets/team/ondrej.jpeg'),
          post: 'Hlavní organizátor - Brno',
          does: 'Meetupy'  
        },
        {
          name: 'Kamil Tomšík',
          img: require('~/assets/team/kamil.jpeg'),
          post: 'Organizátor - Brno',
          does: 'Meetupy'  
        }
      ]
    }
  }  
}
</script>
