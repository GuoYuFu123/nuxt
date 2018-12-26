<template>
 <div>
     <div>
         <img src="~static/1.png" alt="" width="300" height="100">
         <div class="diss">

         </div>
     </div>
     <ul>
         <li>
             <a href="/">home</a>
             <nuxt-link :to="{ name: 'index'}">home--nuxt</nuxt-link>
         </li>
         <li>
             <a href="/about">about</a>
             <nuxt-link :to="{ name: 'about'}">about--nuxt</nuxt-link>
         </li>
         <li>
             <a href="/news">news</a>
             <nuxt-link :to="{ name: 'news', params: {id: '1213'}}">news---nuxt</nuxt-link>
         </li>
         <li>
             <nuxt-link :to="{ name: 'asyncData'}">asyncData</nuxt-link>
         </li>
     </ul>
 </div>
</template>

<script>

export default {
  components: {

  }
}
</script>

<style lang='css'>
.diss {
    width: 300px;
    height: 100px;
    background: url('~static/1.png')
}
</style>

