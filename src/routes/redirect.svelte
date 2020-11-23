<script context="module">
	export async function preload() {
    const fs = await import("fs");

    return {dir: fs.readdirSync('.')};
	}
</script>

<script>
  export let dir;
</script>

{dir}
