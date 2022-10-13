<template>
  
  <web-banner
    :banData="banData" @click="modalView=true"></web-banner>
  <web-modal :mView="modalView" @mClose="modalView=false"></web-modal>
 
</template>

<script>
import webBanner from "@/components/WebBanner.vue"
import webModal from "@/components/WebModal.vue"
import banData1 from "@/data/directs.js"


export default {
  components:{
    webBanner,
    webModal
  },
  data(){
    return {
      banData:banData1,
      modalView:false,
    }
  },
}
</script>

<style>
@import url(./assets/style.css);

</style>