<template>
    <div :style="square" @click="squareClick()"></div>
</template>

<script lang="js">

  export default  {
    name: 'square',
    props: [
      'index',
      'square','fsquare', 
      'mensajes','fmensajes',
      'pickedColor','setAllColorsTo'
    ],
    mounted () {

    },
    data () {
      return {

      }
    },
    methods: {
      squareClick(){
        var clickedColor = this.square.backgroundColor;
        if (clickedColor === this.pickedColor) {
          this.fmensajes.messageDisplay("Elegiste el correcto!");
          this.setAllColorsTo(this.pickedColor);
          this.fmensajes.restartButton("Jugar otra vez!");
          this.fmensajes.headerColor(this.pickedColor);
        } else {
          this.fsquare.backgroundColor(this.index,"#232323");
          this.fmensajes.messageDisplay("Intenta de nuevo!");
        }
      }
    },
    computed: {

    }
} 


</script>

