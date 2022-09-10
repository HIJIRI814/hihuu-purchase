<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
</script>

<template>
  <div class="container">
    <div class="box">
      <h1 style="grid-area: title">見てくれてアリガトー！</h1>
      <div style="grid-area: text">
        <p>
          わざわざQRコードから来てくれてありがとうございます。<br />
          Vol.1, Vol.2
          両方手に入れたかな？持ってるよ！って人はほんとありがとう！！<br />
          まだ持ってない方もぜひもう片方のアルバムもチェックしてみてね！！<br />
          委託もあるぞ！<br />
          続報はYouTube,ニコニコ動画の動画説明欄、IbEthics公式・がむのツイッターをチェック！！
        </p>
        <p>
          <a
            href="https://www.melonbooks.co.jp/detail/detail.php?product_id=1628655"
            >Vol.1委託はこちら</a
          ><br />
          <a
            href="https://www.melonbooks.co.jp/detail/detail.php?product_id=1628656"
            >Vo.2委託はこちら</a
          ><br />
          <a
            href="https://www.melonbooks.co.jp/detail/detail.php?product_id=1634085"
            >両方持ってないのになぜかこのページに来れた人はこちら</a
          >
        </p>
      </div>
      <img src="/img/mary.png" alt="" class="mary" style="grid-area: char1" />
      <img src="/img/renko.png" alt="" class="renko" style="grid-area: char2" />
      <div class="video" style="grid-area: movie">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/UZLR1ynbHwc"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </div>
</template>

<style scoped>
h1 {
  margin: 0;
  text-align: center;
}

p {
  line-height: 1.5;
}

.container {
  width: 100vw;
  height: 100vh;
}

.box {
  width: 80%;
  margin: 32px auto;
  display: grid;
  gap: 24px 12px;
  grid-template:
    "title title title" auto
    "char1 text char2" auto
    "movie movie movie" auto / 250px 1fr 250px;
}

.video {
  position: relative;
  width: 100%;
  height: 0;
  padding-top: 56.25%;
}

.video iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
img {
  width: 100%;
}

@media (max-width: 820px) {
  .box {
    grid-template:
      "title title" auto
      "char1 char2" auto
      "text  text " auto
      "movie movie" auto / 1fr 1fr;
  }
}
</style>
