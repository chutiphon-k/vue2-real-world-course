<template>
	<div>
		<img class='ui circular image' :src="profile.photo" v-if='profile.photo'>
		<h4>Name:</h4> {{ profile.name | upper  }}
		<h4>Description:</h4> {{ profile.description }}
	</div>
</template>

<style>
	img.circular.image {
		width: 120px;
		height: 120px;
	}
</style>

<script>
	export default {
		props: ['profile']
	}
</script>