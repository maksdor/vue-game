<template>
  <div>
    <img src="https://play-lh.googleusercontent.com/LByrur1mTmPeNr0ljI-uAUcct1rzmTve5Esau1SwoAzjBXQUby6uHIfHbF9TAT51mgHm"> 
    <h1>Game</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque, id vitae necessitatibus quidem, 
      recusandae nihil voluptatibus voluptate eos repellat delectus sit labore, culpa dignissimos fugit eum iusto ducimus! 
      Ea, doloribus.</p>
    <nav>
      <i class ="fas fa-desktop"></i>
      <h4>windows</h4>
    </nav>
    <nav>
      <i class ="far fa-clock"></i>
      <h4>date</h4>
    </nav>
    <router-link to="/">Подробнее</router-link>
  </div>
</template>

<style scoped>
div {
  width: 500px  ;
  padding: 10px;
  display: flex;
  flex-direction: column;
  background: #121738;
  color: #D1BDFF;
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
  background: #000000;
  color: #FF89B5;
  font-size: 24px;
  padding: 10px 20px;
  margin-left: auto;
  border-radius: 10px;
  text-decoration: none;
}
</style>