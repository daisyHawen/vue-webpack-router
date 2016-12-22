<template>
    <div>
		<h1>{{header}}</h1>
		<p>{{msg}}</p>
		<div>
		    <audio controls="controls" autoplay="autoplay">
            <source src="../assets/1.mp3" type="audio/mpeg" />
            Your browser does not support the audio element.
            </audio>
		</div>
	</div>
</template>

<script>
	export default {
		data: function() {
			return {
				header:'Hello',
				msg: 'music'
			}
		},
		methods: {
   
        },
	}
</script>