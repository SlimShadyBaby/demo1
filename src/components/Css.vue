<template>
    <div>
        <h1>----css绑定</h1>
        <div class="default" :class="{c1: c1Enable, c2:c2Enable}">对象语法</div>
    </div>
</template>

<script>
export default {
    name: 'Css',
    data() {
        return {
            c1Enable: true,
            c2Enable: false,
            class3: 'c3',
            class4: 'c4'
        }
    }

}
</script>

<style scoped>
    .c1{
        color: red;
    }

    .c2{
        color: yellow;
    }

    .default{
        border-width: 5px;
        border-style: solid;
        border-color: blueviolet;
    }
</style>