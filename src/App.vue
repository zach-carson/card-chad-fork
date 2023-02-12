<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<script setup>
import HelloWorld from './components/HelloWorld.vue'

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style>

.card
{
  background-color: grey;
  border: solid black;
  width: 400px;
  display: inline-flex;
}

.btn { 
  border: 2px solid blue;
  text-transform: uppercase;
  padding: 2px 2px;
  background-color: white;
  font-size: 12px;
  text-align: center;
  margin: auto;
  display: flex;
  display: center;
}

.title-header
{
  text-align: center;
}

.desc
{
  text-align: center;
  display: none;
}


@media screen and (min-width: 500px) and (max-width: 800px)
{
  .btn
  {
    display: none;
  }
}

@media screen and (max-width: 500px)
{
  
  .card
  {
    scale: 0.7;
  }
  
  .img
  {
    scale: 0.6;
  }
 
}

.img {
  width: 400px;
}

.duplicate:hover {
  background-color: yellow;
}

.duplicate:focus {
  background-color: yellow;
}

</style>
