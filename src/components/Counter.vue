<template>
  <div class="text-center">
    <v-btn v-on:click="counter++" rounded v-bind:color="color" dark><slot></slot> {{ counter }} </v-btn>
    {{color}}
  </div>  
  
  <!-- <div></div> -->

</template>


<script>
export default {
  name: 'Counter',
  props:
    {
        color:String
    },
  data: () => ({
    counter : 0,
  })
}
</script>