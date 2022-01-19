<template>
  <div class="card">
    <img :src="image" alt="equilibrium" srcset="" />

    <h1>{{ name }}</h1>

    <h4 class="color1">
      {{ description }}
    </h4>

    <div class="price-time">
      <span>
        <svg width="11" height="18" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M11 10.216 5.5 18 0 10.216l5.5 3.263 5.5-3.262ZM5.5 0l5.496 9.169L5.5 12.43 0 9.17 5.5 0Z"
            fill="#00FFF8"
          />
        </svg>
        <b class="color2">{{ price }}</b>
      </span>

      <span id="time">
        <svg width="17" height="17" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M8.305 2.007a6.667 6.667 0 1 0 0 13.334 6.667 6.667 0 0 0 0-13.334Zm2.667 7.334H8.305a.667.667 0 0 1-.667-.667V6.007a.667.667 0 0 1 1.334 0v2h2a.667.667 0 0 1 0 1.334Z"
            fill="#8BACD9"
          />
        </svg>
        <span class="color1">{{ time }}</span>
      </span>
    </div>

    <hr />

    <div class="creator">
      <img :src="user" alt="avatar" srcset="" />
      <span>
        <span class="color1"> Creation of </span>
        <b> {{ creator }} </b>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    name: String,
    description: String,
    price: String,
    time: String,
    creator: String,
    image: String,
    user: String,
  },
  data() {},
};
</script>

<style scoped>
.card {
  width: 18.75rem;
  height: 31.875rem;
  background: hsl(216, 50%, 16%);
  padding: 1.25rem;
  border-radius: 0.75rem;

  /* position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%); */

  font-size: 0.78rem;
  box-shadow: 0 0 50px #0005;
}

.card > * {
  margin-top: 1.125em;
  display: relative;
}

.card > img {
  width: 16.25rem;
  height: 16.25rem;
  border-radius: 0.56rem;
  margin: 0;
  object-fit: cover;
}

.card h1 {
  font-size: 1.5em;
}

.color1 {
  color: hsl(215, 51%, 70%);
}

.color2 {
  color: hsl(178, 100%, 50%);
  font-weight: 600;
}

.card h4 {
  font-size: 1.2em;
  font-weight: 300;
}

.price-time {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-size: 1.08em;
}

.price-time span {
  display: flex;
  align-items: center;
  gap: 0.3rem;
}

hr {
  background-color: hsl(215, 32%, 27%);
  width: 100%;
  height: 0.0625rem;
  border: none;
  /* border-radius: 10px; */
  margin: 0.9rem 0;
}

.creator {
  display: flex;
  align-items: center;
  gap: 0.625rem;
  font-size: 1.1em;
  margin-top: 0.56rem;
}

.creator img {
  width: 1.875rem;
  border: solid 0.06rem #fff;
  border-radius: 50%;
}

b {
  font-weight: 400;
}
</style>
