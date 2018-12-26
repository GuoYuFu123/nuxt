<template>
    <div>
        {{age}}
        <h1>年龄：{{info.age}}</h1>
    </div>
</template>
<script>
import axios from 'axios';
export default {
    data() {
        return {
            age: 10,
        }
    },
    asyncData() {
        return axios.get('https://api.myjson.com/bins/opvm0').then(res=> {
            return {info: res.data}
        })
    }
}
</script>
