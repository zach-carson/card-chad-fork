<template>
  <h1>{{ msg }}</h1>

<div class="card" id="card1">
  <div>
  <div class="title-header">
    <h2> Jalen Hurts </h2>
  </div>
  <img class = "img" src="https://th.bing.com/th/id/OIP.NX-MOMDx5uAkx4YnlPWexAHaE7?pid=ImgDet&rs=1" alt="jalen hurts">
  <p class = "desc"> Jalen Hurts is a football player </p>
  <!--<a href="https://hax.psu.edu/">-->
  <button class="btn" id='details'> Details </button>
  </a>
</div>
</div>

<button class="duplicate"> Duplicate card </button>

<button class="newcolor"> Toggle background color </button>
  
<button class="something"> Something else </button>
  
<button class="delete"> Delete last card </button>
  
<div>

  
<div id="destination"></div>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<script>

export default {
  methods: {
    hoover() {
      document.querySelectorAll(".card").forEach((item) => {
        if(!item.classList.contains("hoverCard")){
          item.classList.add("hoverCard");
          console.log(item);
        }
        else{
          item.classList.remove("hoverCard");
          console.log(item);
        }
      });
    },
    
    duplicate() {
      const cloneCard = document.querySelector(".card").cloneNode(true);
      document.body.appendChild(cloneCard);
      console.log(cloneCard);    
    },

    background() {
      document.querySelectorAll(".card").forEach((item) => {
        if(!item.classList.contains("basic")){
          item.classList.add("basic");
          console.log(item);
        }
        else{
          item.classList.remove("basic");
          console.log(item);
        }
      });
    },

    heading() {
      document.querySelectorAll(".title").forEach((item) => {   
        if(item.innerHTML=="something else"){
          item.innerHTML="Chad of Cyber IST";
        }
        else{
          item.innerHTML="something else";
        }
      });
    },

    //Kinda borked rn
    deleter(){
      document.querySelector(".card:last-child").remove();
      console.log(card);
    }
  }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
