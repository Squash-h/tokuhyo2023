<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <footer>
    <div class="foot_wrap">
      <ul>
        <li>
          <a href="https://wasedasuperhero.jimdofree.com/" target="_blank">
            <img
              src="../static/images/HP_logo.png"
              alt="公式ホームページ"
              class="img_radius"
            />
          </a>
        </li>
        <li>
          <a href="https://twitter.com/Waseda_SHT" target="_blank">
            <img src="../static/images/X_logo.png" alt="公式Twitter" />
          </a>
        </li>
        <li>
          <a href="https://www.instagram.com/waseda_sht/" target="_blank">
            <img
              src="../static/images/Instagram_logo.png"
              alt="公式Instagram"
            />
          </a>
        </li>
        <li>
          <a href="http://blog.livedoor.jp/wasedasuperhero/" target="_blank"
            ><img
              src="../static/images/blog_logo.png"
              alt="公式ブログ"
              class="img_radius"
          /></a>
        </li>
        <li>
          <a href="https://wasedasai.net/" target="_blank"
            ><img
              src="../static/images/wasedasai.logo.jpg"
              alt="早稲田祭HP"
              class="img_radius"
          /></a>
        </li>
      </ul>
    </div>
    <div class id="footerBottom">
      <p>©2023 早稲田大学特撮評議会</p>
    </div>
  </footer>
</template>
<style>
footer {
  width: 100%;
  height: 160px;
  border-top: #ffffff 4px solid;
  background-color: #333333;
  position: sticky;
  bottom: 0;
  left: 0;
}
footer img {
  max-width: 60px;
  max-height: 60px;
}
.img_radius {
  border-radius: 10%;
}
.foot_wrap {
  padding: 0 5% 0 5%;
}
.foot_wrap ul {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.foot_wrap li {
  list-style: none;
}

#footerBottom {
  border-top: #ffffff 4px solid;
  text-align: center;
}
#footerBottom p {
  color: #ffffff;
}
</style>
