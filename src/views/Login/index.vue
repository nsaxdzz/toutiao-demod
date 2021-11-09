<template>
  <div>
     <h2>登入页</h2>
     <MyInput :value='user'></MyInput>
    <MyButton @click="loginFn"></MyButton>
    <MyButton  @click="loginFn"  type='primary'>登入</MyButton>
    <MyButton @click="loginFn" type='danger'>注册</MyButton>
  </div>
</template>

<script>
import MyButton from'@/components/MyButton.vue'
import MyInput from'@/components/MyInput.vue'
export default {
    data () {
        return {
               user:{
                   name:'默认用户名'
               }
        }
    },
  components: {
      MyButton,
      MyInput
  },
  methods: {
      loginFn(e){
          console.log(e)
      }
  }
}
</script>

<style>

</style>