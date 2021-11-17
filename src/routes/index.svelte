<script>
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
<style lang="scss">
    $main_clr:tomato;
    img { height: 64px; border: darkgreen 5px solid; }
    h1 { color: $main_clr; font-size: 2em; }
    span { text-decoration: line-through; }
</style>

<h1><span>お{na}べ</span>構文{dot === "." ? "( 'ω')" : dot === ".." ? "('ω' )": dot}</h1>

<button on:click={boo}>boo!!({excl})</button>
<br>
<img src={sbelde} alt="ⓈSBELDE">
<p>{tlykeshy} || -> || {@html tlykeshy}</p>