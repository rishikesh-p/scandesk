<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import ValueProp from "$lib/components/ValueProp.svelte";
  import Features from "$lib/components/Features.svelte";
  import Showcase from "$lib/components/Showcase.svelte";
  import Pricing from "$lib/components/Pricing.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<svelte:head>
  <title>ScanDesk | Beautiful Digital QR Menus</title>
  <meta name="description" content="Turn your menu into a powerful sales machine with ScanDesk's lightning-fast, mobile-first QR menus." />
</svelte:head>

<div class="min-h-screen flex flex-col">
  <Header />
  <main class="flex-1">
    <Hero />
    <ValueProp />
    <Features />
    <Showcase />
    <Pricing />
  </main>
  <Footer />
</div>
