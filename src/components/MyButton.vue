<template>
  <div class='btn'
       @click="btn"
        :class="{
            danger:type === 'danger',
            primary:type === 'primary'
            }"
       >
     
          <slot>按钮</slot>
  </div>
</template>

<script>
export default {
    props:{
         type:String,
    },
    methods: {
        btn(e){
            this.$emit('click',e)
            console.log('你点击了按钮')
        }
    }
}
</script>

<style lang="less" scoped>
.btn{
    width: 318px;
    height: 48px;
    display: flex;
    border-radius: 24px;
    justify-content: center;
    align-items: center;
    color:#ccc;
    font-size: 20px;
    background-color: #666;
    margin: 10px 0;

}
.danger{
    background-color: red;
    color: #fff;
}
.primary{
    background-color: green;
    color: rgb(216, 216, 216);
}
</style>