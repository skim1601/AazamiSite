<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      A breakthrough device that empowers people with dementia. With just a simple command, "I forgot," it replays the last 10 seconds of voice, easing the frustration of forgotten memories. 
    </h3>
  </div>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@500&family=Phudu&display=swap');

h1 {
  font-weight: 500;
  font-size: 3rem;
  top: -10px;
  margin: 3rem 0;
}

h3 {
  font-family: 'DM Sans';
}

.greetings h1 {
  font-family: "Orbitron";
  font-size: min(5rem, 10vw);   
  text-align: center;
	background-image: linear-gradient(90deg, rgb(122, 202, 106),rgb(0, 255, 0));
	background-clip: text;
	-webkit-background-clip: text;
	-moz-background-clip: text;
	-webkit-text-fill-color: transparent; 
	-moz-text-fill-color: transparent;
}
.greetings h3 {
  color: #fff;
  font-size: min(1.5rem, 5vw);   
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
    margin: 0;
  }
}
</style>
