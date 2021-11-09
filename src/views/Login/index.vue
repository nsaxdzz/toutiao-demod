<template>
  <div>
      登入页
    <MyButton @click="loginFn"></MyButton>
    <MyButton  @click="loginFn"  type='primary'>登入</MyButton>
    <MyButton @click="loginFn" type='danger'>注册</MyButton>
  </div>
</template>

<script>
import MyButton from'@/components/MyButton.vue'
export default {
  components: {
      MyButton,
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