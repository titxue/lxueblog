<template>
  <div class="wrapper">
    <header>{{ msg }}</header>
    <main>
      <div class="left">左</div>
      <div class="center">内容</div>
      <div class="right">右</div>
    </main>
    <footer>bottom</footer>
  </div>


  
</template>

<script lang="ts">
import { ref, defineComponent } from 'vue'
export default defineComponent({
  name: 'HelloWorld',
  props: {
    msg: {
      type: String,
      required: true
    }
  },
  setup: () => {
    // const count = ref(0)
    // return { count }
  }
})
</script>

<style scoped>
.wrapper{
  resize: both;
  overflow: hidden;
  /* width: 100500px; */
  height: 100vh;
  border: 1px solid black;
  flex-direction: column;
  display: flex;
  text-align: center;
}
header,footer,.left,.right{
  flex: 0 0 10%;
  border: 1px solid red;
  box-sizing: border-box;
  text-align: center;
}
main{
  flex: 1 1 auto;
  display: flex;

}
.center{
  flex: 1 1 auto;
  text-align: center;
}

</style>
