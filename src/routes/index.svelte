<script>
    import mojis  from "./script.js";
    import Kytaa from './Kytaa.svelte';
    const na = mojis[0];
    const sbelde = "https://svelte.jp/svelte-logo-horizontal.svg";
    const tlykeshy = "<strong>AAA</strong>";
    let dot = ".";
    function boo() { dot += "."; }
    $: excl = dot.length;
    $: if(dot.length === 10) {
        alert("BOO!!!!!!!!!!")
    }
</script>

<Kytaa/>
<svelte:head>
    <link rel="stylesheet" href="style.scss"/>
</svelte:head>

<h1><span>お{na}べ</span>構文{dot === "." ? "( 'ω')" : dot === ".." ? "('ω' )": dot}</h1>

<button on:click={boo}>boo!!({excl})</button>
<br>
<img src={sbelde} alt="ⓈSBELDE">
<p>{tlykeshy} || -> || {@html tlykeshy}</p>

<p class="oya">
    <a href="https://discord.gg/7QhMDfyPHR">DISCORD</a>
    <strong>工工工ｴｴｴｴｴｴｪｪｪｪｪｪ(ﾟДﾟ)ｪｪｪｪｪｪｴｴｴｴｴｴ工工工</strong>
</p>
<hr>
<a href="https://discord.gg/7QhMDfyPHR">DISCORD</a>
<strong>工工工ｴｴｴｴｴｴｪｪｪｪｪｪ(ﾟДﾟ)ｪｪｪｪｪｪｴｴｴｴｴｴ工工工</strong>
