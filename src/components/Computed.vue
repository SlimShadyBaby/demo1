<template>
    <div>
        <h1>地址收集</h1>
        省:
        <input type="text" placeholder="请输入省" v-model="province"/> <br />
        市:
        <input type="text" placeholder="请输入市" v-model="city" /> <br />
        区:
        <input type="text" placeholder="请输入市" v-model="area" /> <br />
        详细地址(computed): <span>{{ calAddress }}</span> <br />
        详细地址(watch): <span>{{ address }}</span>
    </div>
</template>

<script>
export default {
    name: 'Address',
    data(){
        return {
            province: '',
            city: '',
            area: '',
            address: ''
        }
    },

    computed: {
        calAddress() {
            return this.province + this.city + this.area
        }
    },

    watch: {
        province: function() {
            this.address = this.province + this.city + this.area
        },
        city: function() {
            this.address = this.province + this.city + this.area
        },
        area: function() {
            this.address = this.province + this.city + this.area
        }
    }
}
</script>
