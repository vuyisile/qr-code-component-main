<template>
  <q-layout view="lHh Lpr lFf"> 
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'
const properties = {
  imgUrl:"images/image-qr-code.png",
  header:"Just Testing",
  paragraph: "This is to just to test the long text, but funny enough, this text is very short and I can't think of something longer (to test with)."

}
const linksList = [
  {
    title:'home',
    route:'/home'
  },
 
]

export default defineComponent({
  name: 'MainLayout',

  components: {
    // EssentialLink,
  },

  data () {
    return {
      leftDrawerOpen: false,
      essentialLinks: linksList
    }
  }
})
</script>
