<script>
import PaddingPane from "../components/PaddingPane.svelte";

</script>
<PaddingPane>
  <h3>半分くらいホント</h3>
  <p class="quoted">ブラウザのクライアントサイドスクリプトとして動作する</p>
  <p>
    →
    <span class="small">ブラウザのクライアントサイドスクリプトとして</span>
    <span class="bold">も</span>
    <span class="small">動作する</span>
  </p>
  <p class="quoted">プログラミング言語（低水準言語）</p>
  <p>→アセンブリなので手でもかけるが殆どC/C++などから生成</p>
</PaddingPane>

<style>
  .quoted {
    font-style: italic;
  }
  .small {
    font-size: calc(var(--slide-width) / 50);
  }
  .bold {
    font-weight: bold;
  }
</style>
