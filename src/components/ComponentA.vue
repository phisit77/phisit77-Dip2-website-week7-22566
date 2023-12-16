<template>
    <div>
        <h1>{{ name }}</h1>
        <p>{{username}}</p>
        <hr />
        <component-b />
    </div>
</template>

<script>
import ComponentB from './ComponentB.vue'
    export default {
         name:'ComponentA',
         inject:['username'],
         components: {
            ComponentB,
         },
    data() {
        return {
            name: "ComponentA"
        }
    },
}
</script>