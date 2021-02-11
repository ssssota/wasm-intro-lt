<script>
  import PaddingPane from "../components/PaddingPane.svelte";
</script>

<PaddingPane>
  <h3>ここがいいぞWASM</h3>
  <p>速い</p>
</PaddingPane>

<style>
  p {
    position: absolute;
    top: 50%;
    left: 50%;
    margin: 0;
    transform: translate(-50%, -50%);
    font-size: calc(var(--slide-width) / 7.5);
    font-weight: bold;
    text-align: center;
  }
</style>
