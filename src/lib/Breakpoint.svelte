<script lang="ts">
	import { dev } from '$app/env';

	export let visible = dev;
</script>

<div class:visible>
	<span>:</span>
</div>

<style lang="postcss">
	div {
		@apply hidden fixed bottom-0 left-0 z-50 m-2 text-sm font-normal;

		& span {
			@apply bg-yellow-500 p-1 text-slate-900 rounded shadow;

			@apply before:content-['xs'];
			@apply sm:before:content-['sm'];
			@apply md:before:content-['md'];
			@apply lg:before:content-['lg'];
			@apply xl:before:content-['xl'];
			@apply 2xl:before:content-['2xl'];
		}

		&.visible {
			@apply block;
		}
	}
</style>
