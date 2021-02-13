<script>
import PaddingPane from "../components/PaddingPane.svelte";

</script>
<PaddingPane>
  <h3>JVM, CLRってなに？</h3>
  <h4>JVM(Java Virtual Machine)</h4>
  <p>JavaやKotlin、Scalaなどから生成されるバイトコード（中間言語）を実行する</p>
  <h4>CLR(Common Language Runtime)</h4>
  <p>C#やF#（、Visual Basic）から生成されるバイトコード（中間言語）を実行する</p>
  <p class="img-wrapper"><img src="./images/jvm.svg" alt="jvm"></p>
</PaddingPane>

<style>
  h4 {
    margin-bottom: 0;
  }
  p {
    margin-top: 0;
  }
  .img-wrapper {
    text-align: center;
  }
  .img-wrapper img {
    width: 50%;
    filter: invert(1);
  }
</style>
