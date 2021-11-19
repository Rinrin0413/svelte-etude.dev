<svelte:head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <meta http-equiv="X-UA-Compatible" content="IE=edge"> <!--対IE-->
    <meta name="format-detection" content="telephone=no"> <!--対電話番号リンク化-->

    <title>Svelte etude|Home</title>
    <meta name="description" content="すべるで">
    <link rel="shortcut icon" href="static/favicon.png">

    <meta property="og:site_name" content="すべるて。">
    <meta property="og:title" content="Home">
    <meta property="og:description" content="すべるで">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://svelte-etude-dev.pages.dev/">
    <meta property="og:image" content="https://svelte-etude-dev.pages.dev/static/favicon.png">
    <meta property="og:locale" content="ja_JP">
    <meta name="twitter:card" content="summary">
    <meta name="twitter:site" content="https://svelte-etude-dev.pages.dev/">
    <meta name="theme-color" content="#FF5722">

    <meta name="title" content="Svelte etude|Home"> <!--検索時用-->
    <meta name="description" content="すべるで">
    <meta name="keywords" content="すべるで">
    <meta name="author" content="@Rinrin_2nd">
    <meta name="copyright" content="©Rinrin_2nd"> 

    <script type="text/javascript" src="src/routes/script.js"></script>
    <link rel="stylesheet" lang="scss" href="src/routes/style.scss">
</svelte:head>
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