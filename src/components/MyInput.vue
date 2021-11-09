<template>
  <input type="text" class="ipt" v-model="value.name">
</template>

<script>
export default {
   props:['value']
}
</script>

<style lang="less" scoped>
.ipt{
    border:none;
    width:318px;
    height: 48px;
    font-size: 20px;
    border-bottom: 2px solid #ccc;
    outline: none;
    margin: 20px auto;
    display: block;
}
</style>