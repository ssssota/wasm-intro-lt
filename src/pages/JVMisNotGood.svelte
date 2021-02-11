<script>
import PaddingPane from "../components/PaddingPane.svelte";

</script>
<PaddingPane>
  <h3>WASM(+WASI)は標準化の動きが強い</h3>
  <p>JVM(GraalVM)はOracleがギチギチに権利を握っている</p>
  <p>WASMはブラウザを作っている企業などが積極的に参加している</p>
  <ul>
    <li>Google</li>
    <li>Microsoft</li>
    <li>Apple</li>
    <li>Mozilla etc...</li>
  </ul>
  <small>参考 <a href="https://www.infoq.com/jp/news/2019/05/wasi-wasm-system-interface/">https://www.infoq.com/jp/news/2019/05/wasi-wasm-system-interface/</a></small>
</PaddingPane>

<style>
  small {
    font-size: calc(var(--slide-width) / 50);
  }
</style>
