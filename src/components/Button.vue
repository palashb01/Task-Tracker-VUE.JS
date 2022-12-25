<template>
    <button :style="{background: color}" class="btn" @click="onClick">{{title}}</button>
</template>

<script>
export default {
    name:'Button',
    props:{
        title:String,
        color:String
    },
  methods:{
      onClick(){
          this.$emit('btn-click')
      }
  }
}
</script>