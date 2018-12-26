<template>
    <div>
        <h1>news pages</h1>
        <ul>
            <li><a href="/">home</a></li>
            <li><nuxt-link :to="{ name: 'index'}">home--nuxt</nuxt-link></li>
            <li>{{$route.params.id}}</li>
            <li><a href="/news/123">news123</a></li>
            <li><a href="/news/456">news456</a></li>
            <li><a href="/news/789">news789</a></li>
            <li><a href="/news/aaa">404</a></li>
            <li><nuxt-link :to='{name: "news-id", params: {id: "12388888", tit: "123"}}'>nuxt-id</nuxt-link></li>
        </ul>
    </div>    
</template>
<script>
    export default {
        transition: 'test'
    }
</script>