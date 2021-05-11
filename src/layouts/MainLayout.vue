<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated color="purple-3">
        <q-toolbar>
            <HeaderContent />
        </q-toolbar>
    </q-header>
    <q-page-container>
        <q-page>
             
        </q-page>
  </q-page-container>
  </q-layout>
</template>
<style lang="scss" scoped>
    .q-header{
       background-color: $deep-orange-13

    }
    .q-toolbar{
        justify-content: flex-end;
    }

</style>  

 
<script>
 

 
import HeaderContent from "../components/header/HeaderContent"

export default {
  name: 'MainLayout' , 
  data () {
    return { 
    }
  },
  components : {HeaderContent}
}
</script>
