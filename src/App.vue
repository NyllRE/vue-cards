<script>
import Card from './components/Card.vue';
export default {
  name: 'App',
  components: { Card },
};
</script>

<template>
  <div class="container">
    <Card
      name="Equilibrium #3429"
      description="Our Equilibrium collection promotes balance and calm."
      price="0.041 ETH"
      time="3 days left"
      creator="Jules Wyvern"
      image="https://github.com/NyllRE/nftchallenge/blob/master/src/images/image-equilibrium.jpg?raw=true"
      user="https://github.com/NyllRE/nftchallenge/blob/master/src/images/image-avatar.png?raw=true"
    />
    <Card
      name="Equibruh lol #9523"
      description="ur money in our pockets nigga fuk u eth millionaires"
      price="69.26 ETH"
      time="54 days left"
      creator="Joe Nutz"
      image="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn.dribbble.com%2Fusers%2F1066740%2Fscreenshots%2F2642237%2Fmain-dribbble.png&f=1&nofb=1"
      user="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.pinimg.com%2F736x%2Fb7%2Fa9%2F1c%2Fb7a91ccaddb1be78835ea844fdb8d239.jpg&f=1&nofb=1"
    />
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-size: 13px;
}

body {
  color: white;
  font-family: 'Outfit', sans-serif;
  background: hsl(217, 54%, 11%);
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
}
</style>
