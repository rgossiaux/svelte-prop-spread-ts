<script lang="ts">
	import Parent from '$lib/Parent.svelte';

	function name() {
		return 'Alice';
	}
</script>

<Parent {name} animal="dog" />
