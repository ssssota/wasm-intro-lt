<script>
  import PaddingPane from "../components/PaddingPane.svelte";
</script>

<PaddingPane>
  <h3>速いだけじゃないWASM</h3>
  <p>ポータブルなバイナリであることを生かして多様なプラットフォームでWASMを動かす</p>
  <h4>WebAssembly System Interface(WASI)</h4>
  <p>要は、WASMにコンパイルしてWindowsでもMacでも動くバイナリが作れる！</p>
  <p class="img-wrapper"><img src="./images/wasm.svg" alt="wasm"></p>
</PaddingPane>

<style>
  .img-wrapper {
    text-align: center;
  }
  .img-wrapper img {
    width: 50%;
    filter: invert(1);
  }
</style>
