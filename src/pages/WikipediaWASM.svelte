<script>
  import CenteringPane from "../components/CenteringPane.svelte";
</script>
<CenteringPane>
  <p>
    WebAssemblyは、<br />
    ウェブブラウザのクライアントサイドスクリプトとして動作する<br />
    プログラミング言語（低水準言語）である。<br />
    <small><a href="https://ja.wikipedia.org/wiki/WebAssembly">Wikipedia</a>より引用</small>
  </p>
</CenteringPane>

<style>
  p {
    font-style: italic;
  }
  p small {
    font-size: calc(var(--slide-width) / 50);
    font-style: normal;
  }
</style>
