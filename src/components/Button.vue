<template>
    <button v-on:click="Onclick()" :style="{background : color}" class="btn">{{text}}</button>
</template>

<script>

export default {
      name : 'Button',
      props : {
          text: String,
          color: String,

    },
     methods : {
         onClick() {
             this.$emit('show-clicked')
        }
    },
}
</script>
