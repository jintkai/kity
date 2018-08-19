<template>
  <Tree :data="data1" @on-select-change="selectChange"></Tree>
</template>
<script>
  export default {
    data () {
      return {
        data1: [
          {
            title: '产品树',
            expand: true,
            children: [
              {
                title: '研发中心',
                expand: true,
                children: [
                  {
                    title: 'Matrix'
                  },
                  {
                    title: 'Norma'
                  }
                ]
              },
              {
                title: '运维中心',
                expand: true,
                children: [
                  {
                    title: 'leaf 1-2-1'
                  },
                  {
                    title: 'leaf 1-2-1'
                  }
                ]
              }
            ]
          }
        ]
      }
    },
    methods:{
      selectChange(n){
        console.log(n)
      }
    }
  }
</script>
