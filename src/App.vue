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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.card{
  border-radius: 24px;
  border: 3px solid #041E42;
  padding: 8px;
  width: 400px;
  display: block;
  margin: auto;
  position: relative;
  overflow: hidden;
  box-shadow: 0px 8px 24px #999;
  background-color: lightgrey;
  text-align: center;
  font-family: Arial, Helvetica, sans-serif;
}

.textbox{
  font-size: 15px;
  margin-left: 112px;
  text-align: right;
  border-radius: 24px;
}

.description{
  text-shadow: -1px 1px 2px #FFFFFF,
				  1px 1px 2px #FFFFFF,
				  1px -1px 0 #FFFFFF,
				  -1px -1px 0 #FFFFFF;
}

.haxbtn{
  display:inline-block;
  text-align: center;
  color: white;
  background-color: #041E42;
  border-radius: 5px;
  font-size: 20px;
  width: 120px;
  height: 32px;
  box-shadow: 0px 10px 24px #999;
  border: 1px solid #041E42;
  visibility: visible;
  padding-top: 10px;
  margin-right: 32px;
}

.haxbtn:hover{
  color: #e0e0e0;
  background-color: #07377a;
  box-shadow: 0px 10px 24px white;
  border: 1px solid #07377a;
}

.haxbtn:focus{
  color: #e0e0e0;
  background-color: #07377a;
  box-shadow: 0px 10px 24px white;
  border: 1px solid #07377a;
}

.title{
  color: white;
  font-size: 24px;
  text-shadow: -1px 1px 2px #000,
				  1px 1px 2px #000,
				  1px -1px 0 #000,
				  -1px -1px 0 #000;
}

.giaImg{
  width: 200px;
  border-radius: 24px;
  box-shadow: 0px 10px 24px #999;
  float: left;
}

.outsideBtn{
  color: white;
  background-color: #041E42;
  border-radius: 5px;
  font-size: 20px;
  width: 120px;
  height: 50px;
  box-shadow: 0px 10px 24px #999;
  border: 1px solid #041E42;
  margin-right: 32px;
  margin-bottom: 16px;
  display: inline-block;
}

.outsideBtn:hover{
  color: #e0e0e0;
  background-color: #07377a;
  box-shadow: 0px 10px 24px white;
  border: 1px solid #07377a;
}

.outsideBtn:focus{
  color: #e0e0e0;
  background-color: #07377a;
  box-shadow: 0px 10px 24px white;
  border: 1px solid #07377a;
}

.basic{
  background-color: hotpink;
}

.hoverCard{
  border: 3px solid purple;
  box-shadow: 0px 8px 24px yellow;
}

input:checked + label + .description { display:none; }



</style>
