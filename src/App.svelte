<script lang="ts">
  import ProgressBar from "./components/ProgressBar.svelte";
  import SlideView from "./components/SlideView.svelte";
  import { page } from "./utils/page";
  import TitlePage from "./pages/TitlePage.svelte";
  import WhoAmI from "./pages/WhoAmI.svelte";
  import WhatIsWasm from "./pages/WhatIsWASM.svelte";
  import WikipediaWasm from "./pages/WikipediaWASM.svelte";
  import Really from "./pages/Really.svelte";
  import WASMHistory from "./pages/WASMHistory.svelte";
  import WhyWasm from "./pages/WhyWASM.svelte";
  import Pros from "./pages/Pros.svelte";
  import Almost from "./pages/Almost.svelte";
  import Truth from "./pages/Truth.svelte";
  import IsThatJvm from "./pages/IsThatJVM.svelte";
  import WhatAreJVMCLR from "./pages/WhatAreJVMCLR.svelte";
  import VeryLike from "./pages/VeryLike.svelte";
  import JVMisNotGood from "./pages/JVMisNotGood.svelte";
  import AltDocker from "./pages/AltDocker.svelte";
  import MaybeDifficult from "./pages/MaybeDifficult.svelte";
  import Languages from "./pages/Languages.svelte";
  import Conclusion from "./pages/Conclusion.svelte";
  export let listView = false;

  const pages = [
    TitlePage,
    WhoAmI,
    WhatIsWasm,
    WikipediaWasm,
    Really,
    WASMHistory,
    WhyWasm,
    Pros,
    Almost,
    Truth,
    IsThatJvm,
    WhatAreJVMCLR,
    VeryLike,
    JVMisNotGood,
    AltDocker,
    MaybeDifficult,
    Languages,
    Conclusion,
    // INSERT YOUR PAGE HERE!
  ];

  const handleKeydown = (e: KeyboardEvent) => {
    switch (e.code) {
      case "ArrowRight":
      case "Space":
      case "Enter":
        page.next();
        break;
      case "ArrowLeft":
        page.prev();
        break;
    }
  };
</script>

<svelte:window on:keydown={handleKeydown} />

{#if !listView}
  <SlideView onLeftClick={page.prev} onRightClick={page.next}>
    <svelte:component this={pages[$page - 1]} />
  </SlideView>
  <ProgressBar progress={($page - 1) / (pages.length - 1)} />
{:else}
  {#each pages as p}
    <SlideView onLeftClick={undefined} onRightClick={undefined}>
      <svelte:component this={p} />
    </SlideView>
  {/each}
{/if}
