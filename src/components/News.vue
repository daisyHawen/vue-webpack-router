<template>
    <div>
    <div>
		<h1>Home</h1>
		<p>{{msg}}</p>
	</div>
	<h1>{{header}}</h1>
	</div>
</template>

<script>
	export default {
		data: function() {
			return {
				header:'News',
				msg: 'Hello, vue router!'
			}
		}
	}
</script>