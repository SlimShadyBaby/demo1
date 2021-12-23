<template>
    <div id="demo">
        <h1 class="first-demo">first component demo {{ title }}</h1>
    </div>
</template>

<script>
export default {
    name: 'Demo',
    data(){
        return {
            title: "beautiful demo"
        }
    },
    created(){
        this.title = this.title + "?"
    }
}
</script>

<style>
    .first-demo{
        color: red;
    }
</style>