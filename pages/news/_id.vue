<template>
    <div>
        <h2>news-content</h2>
        <p>newsIdL {{$route.params.id}}</p>
        <p>tit={{$route.params.tit}}</p>
        <ul>
            <li><a href="/">home</a></li>
        </ul>
    </div>
</template>

<script>
export default {
    validate({params}) {
        return /^\d+$/.test(params.id);
    },
    data() {
        return {
            title: this.$route.params.id
        }
    },
    head() {
        return {
            title: this.title,
            meta: [{
                hid:"dec",
                name: 'news',
                content:'this.is.new.page'
            }]
        }
    }
}
</script>

<style>

</style>
