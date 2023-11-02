<template>
  <q-page>
      <carrousel-component/>
      <normativa-component :normativa="normas"/>
      <div class="flex flex-center">
        <valores-components :valores="valores"/>
      </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import CarrouselComponent from 'src/components/CarrouselComponent.vue';
import ValoresComponents from 'src/components/ValoresComponents.vue';
import NormativaComponent from 'src/components/NormativaComponent.vue';

export default defineComponent({
  name: 'IndexPage',
  components:{
    CarrouselComponent,
    ValoresComponents,
    NormativaComponent
  },
  setup(){
    const valores = [{nombre:'Mision',descripcion:'naguara'},{nombre:'Vision',descripcion:'naguarax2'}]
    const normas = ['hola','soy el mismo']
    return{
      valores,normas
    }
  }
})
</script>
