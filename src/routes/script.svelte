<script>
    import Kytaa from './Kytaa.svelte';
    const na = "那";
    const sbelde = "https://svelte.jp/svelte-logo-horizontal.svg";
    const tlykeshy = "<strong>AAA</strong>";
    let dot = ".";
    function boo() { dot += "."; }
    $: excl = dot.length;
    $: if(dot.length === 10) {
        alert("BOO!!!!!!!!!!")
    }
</script>