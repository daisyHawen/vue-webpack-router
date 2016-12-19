<template>
    <div>
		<h1>{{header}}</h1>
		<p>{{msg}}</p>
		<ul class="list-group">
	        <div class="list-group-item">
			<div class="list_item_content row">
				<div class="WB_screen "></div>
				<div class="WB_face col-sm-2">
					<img src="../assets/x.jpg" height="50" width="50">
				</div>
				<div class="WB_detail col-sm-10">
				    <div class="WB_author">
				    <a>{{item.author}}</a>
				    </div>
					<div class="WB_from">
					<a >{{item.time}}</a>
					</div>
					<div class="WB_text">{{item.info}}</div>
				</div>
			</div>
		    </div>
        </ul>
	
	</div>
</template>
<style>
	.WB_author a{
		color: #333;
		font-weight:700;
		font-size:14px; 
	}
	.WB_from a{
		color: #919191;
		text-decoration: none;
	}
	.WB_text{
		font-size: 14px;
		margin-top: 2px;
		padding-bottom: 0;
	}
</style>
<script>
	export default {
		data: function() {
			return {
				header:'Hello',
				msg: 'Hello, welcom to my blog',
				item:{
					"info":"This is content",
					"time":"20161219",
					"author":"daisyHawen"
				}
			}
		}
	}
</script>