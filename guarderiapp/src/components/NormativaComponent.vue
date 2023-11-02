<template>
  <q-card
    dark bordered class="bg-primary my-card q-ma-md"
  >
    <q-card-section style="text-align: center;">
      <div class="text-h6">Normativa</div>
    </q-card-section>

    <q-separator dark inset />

    <q-card-section>
        <ul>
          <li v-for="(regla,index) in normativa" :key="index">{{ regla }}</li>
        </ul>
    </q-card-section>
  </q-card>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  props:{
    normativa:{
      type:Array
    }
  }
})
</script>
