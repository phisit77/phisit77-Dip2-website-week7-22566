<template>
    <div>
        <h1>{{ name }}</h1>
        <hr/>
        <p>{{username}}</p>
    </div>
</template>

<script>
    export default {
    name:'ComponentC',
    inject:['username'],
    data() {
        return {
            name: "ComponentC"
        }
    },
}
</script>