<template>
  <q-card
    bordered dark class="bg-primary my-card q-ma-xs "
    v-for="(valor,index) in valores" :key="index"
  >
    <q-card-section style="text-align: center;">
      <div class="text-h6">{{valor.nombre}}</div>
    </q-card-section>

    <q-separator dark inset />

    <q-card-section>
      {{ valor.descripcion }}
    </q-card-section>
  </q-card>
</template>
<script>
import { defineComponent } from 'vue';

export default defineComponent({
  props:{
    valores:{
      type: Array,
      required:true
    }
  },
  setup () {
    return {
    }
  }
})
</script>
