<template>
  <div>
    hello info component
    <button type="button" @click="add()">添加</button>
  </div>
</template>

<script>
  import store from '@/store'
  export default {
    name: 'Info',
    store,
    data(){
      return {
        msg:'this is not problem'
      }
    },
    methods:{
      add(){
        debugger;
        console.log('add Event from info!');
        store.commit('increase')
      },
      output(){
        console.log('');
      }
    }
}
</script>

<style scoped>

</style>
