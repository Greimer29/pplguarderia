<template>
  <q-card
    dark bordered class="bg-deep-orange-9 my-card q-mb-xs"
    v-for="(valor,index) in valores" :key="index"
  >
    <q-card-section style="text-align: center;">
      <div class="text-h6">{{valor.nombre}}</div>
      <div class="text-subtitle2">Mision de la institucion</div>
    </q-card-section>

    <q-separator dark inset />

    <q-card-section>
      as;iofjsiofhsfhSLDfjnSLfnsdlfnsldfns
      {{ 2 }}
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
