<template>
	<v-app>
		<div class="loader" :class="{active: active}">
			<div class="loader-content">
				<img src="https://res.cloudinary.com/lukman/image/upload/v1533998020/avatar.png" alt="">
				<v-progress-linear
					background-color="grey lighten-3"
					color="green lighten-1"
					height="10"
					:indeterminate="true"
				></v-progress-linear>
			</div>
		</div>
	</v-app>
</template>

<script>
export default {
	name: 'Loader',
	props: {
		active: {
			type: Boolean,
			default: true
		}
	}
}
</script>
