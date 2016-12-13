<template>
<div>
	<ul>
		<li v-for="news in newsList">
            <router-link :to="{ name: 'detail', params: { id: news.id}, query: { info: news.query } }">{{news.title}}</router-link>
		</li>
	</ul>
	<div>
		<router-view></router-view>
	</div>
</div>
</template>

<script>	
	export default{
		data: function(){
			return {
				newsList: [
					{ id: '01', title: 'News 01',query:'xyx'},
					{ id: '02', title: 'News 02'},
					{ id: '03', title: 'News 03'}
				]
			}
		}
	}	
</script>