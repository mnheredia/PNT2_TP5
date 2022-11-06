<template>
    <div id="navigator">
			<button id="reset" @click="reset()"> {{ restartButton }}</button>
			<span id="message"> {{ messageDisplay }}</span>

			<button id="easy" @click="easy()" :class="{'selected': !isHard}">Facil</button>
			<button id="hard" @click="hard()" :class="{'selected': isHard}">Dificil</button>
		</div>
</template>

<script>

  export default  {
    name: 'navigator',
    props: ['reset','easy','hard','restartButton','messageDisplay','isHard'],
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
 
