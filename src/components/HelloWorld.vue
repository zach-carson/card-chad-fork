<template>
  <h1>{{ msg }}</h1>

<!-- My custom code -->
<button id="duplicate" class="outsideBtn" v-on:click="duplicate">Duplicate</button>
<button id="bg" class="outsideBtn" v-on:click="background">Background</button>
<button id="header" class="outsideBtn" v-on:click="heading">Heading</button>
<button id="delete" class="outsideBtn" v-on:click="delete">Delete</button>

<div class="card">
  <h1 class="title">Chad of Cyber IST</h1>

  <img class="giaImg" src="https://media.discordapp.net/attachments/963095262363017246/1020131830323744788/unknown.png?width=468&height=468" alt="Professor Giacobe">
  
<div class="textbox">
  <details>
    <summary class="haxbtn">Details</summary>
    <p class="description pScale">Professor Giacobe may look like a simple man but perceptions can be misleading. Underneath the facade of a simple college of IST professor lies the holiness of an <strong>IST GOD</strong>!</p>
  </details>

  </div>
</div>


  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <button type="button" @click="state.count++">count is: {{ state.count }}</button>
  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
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
      if(document.querySelector(".title").innerHTML=="something else"){
        document.querySelector(".title").innerHTML="Chad of Cyber IST";
      }
      else{
        document.querySelector(".title").innerHTML="something else";
      }
    },
    
    //Kinda borked rn
    delete(){
      const card = document.querySelectorAll(".card");
      const last = card[card.length-1];
      last.remove();
      console.log(last);
    }
  }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
