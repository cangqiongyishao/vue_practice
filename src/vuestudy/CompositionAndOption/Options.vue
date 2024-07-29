<template>
    <div>
        <button @click="onUpdateCount">Cnt:{{ count }}</button>
    </div>
</template>

<script>
export default {
    name:'Options',
    data(){
        return {
            count:0
        }
    },
    methods:{
        onUpdateCount(){
            this.count++;
        }
    }

}
</script>

<style scoped>
/* 可以在这里添加样式 */
</style>