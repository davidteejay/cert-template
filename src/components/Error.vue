<template>
	<v-app>
		<div class="error-container">
			<div class="bg"></div>
			<div class="content">
				<h1>Oops!!!</h1>
				<h2>An error occurred while trying to load this page</h2>
				<p @click="reload">
					<i class="material-icons">refresh</i>
					<span> TRY AGAIN</span>
				</p>
			</div>
			
		</div>
	</v-app>
</template>

<script>
export default {
	name: 'Error',
	methods: {
		reload: function(){
			window.location.reload()
		}
	}
}
</script>
