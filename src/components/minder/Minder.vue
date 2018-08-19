<template>
  <div>
    <iframe :src="'../../static/kityminder-editor/dist/index.html?id='+this.minderId"
            style="width: 100%;height:100%;"></iframe>
  </div>
</template>

<script>
  export default {
    props: {
      id: {
        type: String,
        required: true
      }
    },
    watch:{
      id(nv){
        this.minderId = nv
      }
    },
    name: "Minder",
    data(){
      return {
        minderId:this.id
      }
    }
  }
</script>

<style scoped>

</style>
