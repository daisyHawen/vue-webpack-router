<template>
    <div>
	<div>
		<h1>Home</h1>
		<p>{{msg}}</p>
	</div>
	<div>
		<ul class="nav nav-tabs">
			<li>
                <router-link  to="/Home/news">News</router-link>
			</li>
			<li>
			    <router-link  to="/Home/message">Message</router-link>	
			</li>
		</ul>
		<router-view></router-view>
	</div>
	</div>
</template>

<script>
	export default {
		data: function() {
			return {
				msg: 'Hello, vue router!'
			}
		}
	}
</script>