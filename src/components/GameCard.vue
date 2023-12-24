<script setup>
defineProps ({
  game: {
    type: Object,
    default: {
      id: 1,
      title: 'Game',
      short_description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem eos numquam, tempora quibusdam maxime distinctio consequatur enim rerum sunt perferendis nostrum corporis debitis ab iste amet, modi veniam impedit inventore?',
      release_date: '11.02.2003',
      platform: 'Windows',
      thumbnail: "https://play-lh.googleusercontent.com/LByrur1mTmPeNr0ljI-uAUcct1rzmTve5Esau1SwoAzjBXQUby6uHIfHbF9TAT51mgHm",
    },
  },
});
</script>

<template>
  <div>
      <img :src="game.thumbnail"/> 
      <h1>
        {{game.title}}
      </h1>
      <p>
        {{game.short_description}}
      </p>
      <nav>
        <i class ="fas fa-desktop"></i>
        <h4>{{game.platform}}</h4>
      </nav>
      <nav>
        <i class ="far fa-clock"></i>
        <h4>{{game.release_date}}</h4>
      </nav>
      <router-link :to="{ name: 'detail', params: { id: game.id } }">
        See more
      </router-link>
  </div>
</template>

<style scoped>

div {
  width: 100%;
  padding: 10px;
  display: flex;
  flex-direction: column;
  background: #111111;
  color: #E5E4E2;
  border-radius: 10px;
}

img {
  width: 100%;
  aspect-ratio: 16/9;
  border-radius: 10px;
}

h1 {
  font-size: 30px;
  margin-top: 20px;
}

p {
  font-size: 20px;
  margin-top: 20px;
  line-height: 120%;
}

nav {
  display: flex;
  margin-top: 20px
}

h4, i {
  font-size: 20px;
  margin-right: 10px
}

a {
  background: #BEBFC5;
  color: #353839;
  font-size: 24px;
  padding: 10px 20px;
  margin-left: auto;
  border-radius: 10px;
  text-decoration: none;
}
</style>