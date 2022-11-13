<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>hola mundo</h1>
    <Button @click="goToDaybook" class="btn btn-primary">primary</Button>
    <Button @click="goToDaybook" class="btn btn-secondary">secondary</Button>
    <Button @click="goToDaybook" class="btn btn-success">success</Button>
  </div>
</template>

<script>
export default{
  methods:{
    goToDaybook(){
      this.$router.push({name: 'no-entry'})
    }
  }
}
</script>
