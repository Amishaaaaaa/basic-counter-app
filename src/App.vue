<!-- Composition api -->
<script setup>
  import { ref } from "vue";
  const count = ref(0);

  const addToCount = () => {
    count.value = count.value + 1;
  }
  const subtractFromCount = () => {
    count.value = count.value - 1;
  }
</script>

  
<template>
  <main>
    <div>
      <h4>
      The current count is...
      </h4>
      <h1>{{ count }}</h1>
      <button @click="subtractFromCount()">-</button>
      <button @click="addToCount()">+</button>
    </div>
  </main>
</template>
 


<style scoped>
  main {
    background-color: rgb(174, 205, 227);
    height: 100vh;
    width: 100vw;
    display:flex;
    align-items: center;
    justify-content: center;
  }
  div {
    display:flexbox;
    align-items: center;
    justify-content: center;
    text-align: center;
    background-color: rgb(205, 79, 79);
    height: 50vh;
    width: 80vh;
    border-radius: 2vh;
  } 
  h4 {
    margin-top: 3vh;
    font-size: 5vh;
  }
  h1 {
    font-size: 15vh;
  }
  button {
    padding: 2vh;
    font-size: 4vh;
    width: 20vh;
    border-radius: 3vh;
    background-color: aliceblue;
  }
</style>




<!-- options api -->
<!-- <script>
  export default({
    data(){
      return {
        count:0
      }
    },
    methods: {
      addToCount() {
        this.count = this.count + 1;
      },
      subtractFromCount() {
        this.count = this.count - 1;
      }
    }
  })
</script> -->