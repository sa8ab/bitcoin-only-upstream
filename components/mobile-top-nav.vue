<template>
	<div
		id="mobile-top-navigation"
		:class="{ 'mobile-side-nav-open': showMobileSideNav }"
	>
		<div class="mobile-menu-toggle">
			<input type="checkbox" v-model="showMobileSideNav" />
			<span></span>
			<span></span>
			<span></span>
		</div>

		<div class="logo">
			<nuxt-link to="/">
				<img src="/bitcoin-only-logo.png" alt="Bitcoin Only" />
			</nuxt-link>
		</div>
	</div>
</template>

<style lang="scss" scoped>
@import "assets/css/mobile-top-nav.scss";
</style>

<script setup lang="ts">
import { useState } from "nuxt/app";

const showMobileSideNav = useState("showMobileSideNav", () => false);
</script>
