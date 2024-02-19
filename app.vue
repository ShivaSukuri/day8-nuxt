<template>
  <div>
  <div >
    <ul class="nav">
    <NuxtLink to="/">index</NuxtLink>
    <NuxtLink to="/Home">Home</NuxtLink>
    </ul>
  </div>
  <!-- <NavHeader /> -->
<!-- <counter /> -->
 <NuxtPage />  
<!-- <a href="#" @click="view('Welcome')">Home</a>
<a href="#" @click="view('counter')">Counter</a>
<welcome v-if="name==='Welcome'" />
<counter v-if="name==='counter'" />  -->
<Counter />
  </div>
</template>

<script setup>
const name=ref('Welcome')
 const view=(name1)=>{
name.value=name1;
 }
</script>

<style lang="scss" scoped>
.nav{
  background-color: rgb(221, 170, 134);
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 70px;
  text-decoration: none;
}

</style>