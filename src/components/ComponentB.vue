<template>
    <div>
        <h1>{{ name }}</h1>
        <p>{{employee}}</p>
        <component-c />
    </div>
</template>

<script>
import ComponentC from './ComponentC.vue'
    export default {
    name:'ComponentB',
    inject : ['employee'],
    components: {
        ComponentC,
    },
    data() {
        return {
            name: "ComponentB"
        }
    },
}
</script>