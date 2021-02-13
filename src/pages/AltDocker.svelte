<script>
  import PaddingPane from "../components/PaddingPane.svelte";
</script>

<PaddingPane>
  <h3>Dockerをも置き換える？</h3>
  <p>Docker社の創業者が「2008年にWASM+WASIがあればDockerを開発する必要はなかった」と言っている。(2019)</p>
  <p>モダンブラウザを中心にWASIの実装が進んでいる</p>
  <ul>
    <li>Chrome / Firefox / Safari</li>
    <li>Wasmtime / Wasmer / Node.js</li>
  </ul>
  <p class="img-wrapper"><img src="./images/docker.svg" alt="docker"></p>
  <small>参考 <a href="https://thinkit.co.jp/article/17486">https://thinkit.co.jp/article/17486</a></small>
</PaddingPane>

<style>
  ul {
    margin: 0;
  }
  .img-wrapper {
    text-align: center;
    margin-bottom: 0;
  }
  .img-wrapper img {
    width: 50%;
    filter: invert(1);
  }
  small {
    font-size: calc(var(--slide-width) / 50);
  }
</style>
