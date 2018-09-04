<template>
	<div>
		<b-embed type="iframe"
          aspect="1by1"
          src="http://m.hani.co.kr"
          allowfullscreen
          id="left"
  		></b-embed>
  	</div>
</template>


<script type="text/javascript">
	import Vue from 'vue'
	new Vue({
		el: '#left',
		beforeCreate : function(){
			console.log("***************beforeCreate**************");
		},
		created: function(){
			console.log("****************Created****************");
		},
		mounted : function(){
			console.log(document.getElementById('left').src);
		},
		updated : function(){
			console.log("******************updated*************");
		}
	})
	export default{
	}

</script>

<style type="text/css">

</style>
