<template>
  <div class="entry-title d-flex justify-content-between p-2">

    <div>
        <span class="text-success fs-3 fw-bold">15</span>
        <span class="fs-3 mx-1">julio</span>
        <span class="mx-2 fs-4 fw-ligth">2022, jueves</span>
    </div>

    <div>
        <button class="btn btn-danger mx-2">
            Borrar
            <i class="fa fa-trash-alt"></i>
        </button>
        <button class="btn btn-primary">
            Subir Foto
            <i class="fa fa-upload"></i>
        </button>
    </div>
  </div>

  <hr>
  <div class="d-flex flex-column px-3 h-75">
    <textarea placeholder="¿Que sucedio hoy?"></textarea>
  </div>
  <Fab icon="fa-save"></Fab>
  <img src="https://alfabetajuega.com/hero/2021/08/final.jpg" alt="imagen-entry" class="img-thumbnail">
</template>

<script>
import {defineAsyncComponent} from 'vue'
export default {

    components:{
        Fab: defineAsyncComponent(()=>import('@/modules/daybook/components/Fab.vue'))
    }
}
</script>

<style scoped lang="scss">
textarea{
    font-size: 20px;
    border: none;
    height: 100%;
    &:focus{
        outline: none;
    }
}
img{
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
}
</style>