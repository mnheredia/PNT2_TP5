<template>
    <div id="header" :style="{backgroundColor: color}">
      <h1>TP5 <br>
        <span id="colorDisplay">{{pickedColor}}</span>
        <br>
        Adivina el color!</h1>
		</div>
</template>

<script lang="js">

  export default  {
    name: 'header',
    props: ['color','pickedColor'],
    mounted () {

    },
    data () {
      return {

      }
    },
    methods: {

    },
    computed: {

    }
}


</script>
