<svelte:head>
    <title>Svelte etude|Home</title> <!--Tab表示用-->
    <meta name="title" content="Svelte etude|Home"> <!--検索時用-->
    <meta name="description" content="すべるで">

    <meta property="og:title" content="Home">
	<meta property="og:description" content="すべるで">
    <meta property="og:url" content="https://svelte-etude-dev.pages.dev/">
    <meta property="og:type" content="website"> <!-- website or article -->
    <style lang="scss">@import "../../static/style/style.scss";</style>
    <script type="text/javascript" src="../../static/script/script.js"></script>
</svelte:head>

<script>
    import mojis  from "../../static/script/script.js";
    import Kytaa from './Kytaa.svelte';
    const na = mojis[1];
    const sbelde =mojis[7];
    const tlykeshy = mojis[8];
    let dot = ".";
    function boo() { dot += "."; }
    $: excl = dot.length;
    $: if(dot.length === 10) {
        alert("BOO!!!!!!!!!!")
    }
</script>

<Kytaa/>

<h1><span>お</span></h1>
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
