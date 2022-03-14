<template>
<div>
    <p>{{ text }}</p>
<a :href="link">Daily Dev</a><br/>
<button @click="newText" >Say "hi"</button>
<input v-model="text" type="text" />
</div>
</template>

<script>
import Navbar from "./components/Navbar.vue"
export default {
components: {
  Navbar
},
data(){
  return {
text: "Vue rocks",
link: "https://daily.dev"
  };
},
methods: {
hola() {
  console.log("Hi")
},
newText() {
  this.text = ""
}

}
}
</script>

<style>

</style>