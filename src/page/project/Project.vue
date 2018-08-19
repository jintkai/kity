<template>
  <div class="project">
    <project-tree></project-tree>
    <div style="flex:1;">
      <minder style="height:100%;" id="1"></minder>
    </div>
  </div>
</template>

<script>
  import ProjectTree from './ProjectTree'
  import Minder from "../../components/minder/Minder";

  export default {
    name: "Project",
    components: {
      Minder,
      ProjectTree
    }
  }
</script>

<style scoped>

  .project {
    display: flex;
    height: 500px;
  }
</style>
