<template>
  <div>

    <Head>
      <!-- Primary Meta Tags -->
      <Title>{{ pageTitle }}</Title>
      <Meta name="title" :content="title" />
      <Meta name="description" :content="description" />

      <!-- Open Graph / Facebook -->
      <Meta property="og:type" content="website" />
      <Meta property="og:url" content="https://sitcon.org/2022/cfp/" />
      <Meta property="og:site_name" content="SITCON 2022" />
      <Meta property="og:title" :content="title" />
      <Meta property="og:description" :content="description" />
      <Meta property="og:image" :content="image" />

      <!-- Twitter -->
      <Meta property="twitter:card" content="summary_large_image" />
      <Meta property="twitter:url" content="https://sitcon.org/2022/cfp/" />
      <Meta property="twitter:title" :content="title" />
      <Meta property="twitter:description" :content="description" />
      <Meta property="twitter:image" :content="image" />

      <!-- Icon -->
      <Link rel="icon" href="https://sitcon.org/2022/imgs/cfp/CFP_favicon.ico" sizes="any" />
      <Link rel="icon" href="https://sitcon.org/2022/imgs/cfp/CFP_favicon.png" sizes="any" />
      <Link rel="icon" href="https://sitcon.org/2022/imgs/cfp/CFP_favicon.svg" type="image/svg+xml" />
    </Head>
    <div class="cfp-main-page">
      <div class="cfp-container">
        <div class="logos">
          <logo-sitcon />
          <logo-cat-in-a-maze />
        </div>
        <h1 class="call-for-paper">
          <div class="corner" />
          <div class="corner" />
          <div class="corner" />
          <div class="corner" />
          稿件徵求中！
        </h1>
        <cfp-date-links />
      </div>
      <cfp-rounded-glass-box>
        <h3>關於 SITCON</h3>
        <p>SITCON 學生計算機年會自 2013 年發起，以學生為本、由學生自發舉辦，長期投身學生資訊教育與推廣開源精神，希望引領更多學子踏入資訊的殿堂，更冀望所有對資訊有興趣的學生，能夠在年會裏齊聚一堂，彼此激盪、傳承、啟發，達到「學以致用、教學相長」的實際展現。</p>
        <p>在 SITCON 的第 X 週年，期望我們秉持初衷——讓學生們分享與交流知識，把各地學生串連起來的 X 字路口——也期望每人皆能在與大家的聊天與討論之中，找到自己的方向、熱情。</p>
        <h3>SITCON 歷年網站</h3>
        <div class="prev-sites">
          <cfp-prev-site src="/2022/imgs/cfp/prev-sites/2021.png" href="https://sitcon.org/2021/">SITCON 2021</cfp-prev-site>
          <cfp-prev-site src="/2022/imgs/cfp/prev-sites/2020.png" href="https://sitcon.org/2020/">SITCON 2020</cfp-prev-site>
          <cfp-prev-site src="/2022/imgs/cfp/prev-sites/2019.png" href="https://sitcon.org/2019/">SITCON 2019</cfp-prev-site>
          <cfp-prev-site src="/2022/imgs/cfp/prev-sites/2018.png" href="https://sitcon.org/2018/">SITCON 2018</cfp-prev-site>
        </div>
        <h3>參與討論</h3>
        <p>SITCON 是個開放的社群，許多籌備的相關事項都會在公開的郵件論壇上進行討論，如果有興趣參與，歡迎訂閱 SITCON 的郵件論壇並貢獻你的想法！</p>
        <p>若你想進一步了解過往討論的內容，也歡迎到 GitLab 上查看 SITCON 2022 的籌備歷程。</p>
        <div class="rad-btns">
          <cfp-rad-btn href="https://groups.google.com/g/sitcon-general/" content="SITCON 郵件論壇" />
          <cfp-rad-btn href="https://gitlab.com/sitcon-tw/2022/2022-board/-/issues" content="籌備歷程紀錄" />
        </div>
      </cfp-rounded-glass-box>

      <cfp-rounded-glass-box class="cat-background">
        <h3 class="margin-0">2022 年會主題</h3>
        <h1 class="margin-0">Cat in a Maze</h1>
        <p>Cat in a Maze 參考自 Rat in a Maze 這道經典演算法題目。題目描述一隻老鼠要走迷宮，在給定了迷宮形狀的前提下，要努力找出走出迷宮的出路。「Rat in a
          Maze」這句話切實地反映了劇烈動盪時代下的學生們在面對未來的生涯發展時，猶如一隻無法逃避、勢必得進入體制這一迷宮的老鼠。</p>
        <h3 class="text-center">但是⋯⋯我們真的只能當老鼠嗎？</h3>
        <p>不如，像貓咪一樣思考？以貓咪的個性，第一直覺想到的會是遇到迷宮時，直接破壞迷宮離開，或者是使用我們想不到的方式解決迷宮。同時貓咪相較於老鼠，對一切事物充滿好奇、敢於探索未知事物，不畏強權挑戰一切，是貓咪獨特的個性。<br>
          對於學生而言，充滿好奇、敢於探索未知事物相當重要，畢竟自己的未來要由自己來定義。當大家陷入迷惘的時候，比起使用老鼠告訴大家已經陷入迷惘了，不如讓我們可以看看貓咪、學學貓咪，換個思維邏輯去面對迷惘的現況，保持著好奇心與探索的樂趣。又或者跳脫框架，創造屬於自己的美好未來。</p>
        <h3 id="request-for-sponsorship"><a href="#request-for-sponsorship"></a>SITCON 贊助徵求</h3>
        <p>SITCON 的舉辦，除了有賴眾多志工的努力，也需要金錢的支持。<br>如果您認同 SITCON 的理念，歡迎以行動支持 SITCON 的運作，讓更多交流產生！</p>
        <p>企業合作歡迎聯繫 <a href="mailto:contact@sitcon.org">contact@sitcon.org</a></p>
        <div class="rad-btns">
          <cfp-rad-btn href="https://ocf.neticrm.tw/civicrm/contribute/transact?reset=1&id=55" content="個人贊助方案" />
        </div>
      </cfp-rounded-glass-box>

      <Footer />
    </div>
  </div>
</template>
<script setup>
const pageTitle = ref('Call for Papers')
const title = ref('SITCON X - Cat in a Maze')
const description = ref('在 SITCON 的第 X 週年，期望我們秉持初衷——讓學生們分享與交流知識，把各地學生串連起來的 X 字路口——也期望每個人能夠向貓咪學習，保持著好奇心與探索的樂趣，跳脫原有的思維邏輯與框架，創造屬於自己的美好未來！')
const image = ref('https://sitcon.org/2022/imgs/cfp/cfp-og.png')
</script>
<style lang="sass" scoped>

.cfp-main-page
  background-image: url(/imgs/cfp/CFP_desktop_mainPage.jpg)
  background-position: top -12vw center
  background-size: cover
  background-color: black
  background-repeat: no-repeat
  @media screen and (max-width: 768px)
    background-position: top 50px center
    background-image: url(/imgs/cfp/CFP_mobile_mainpage.jpg)
.cfp-container
  padding-top: 64px
  @media screen and (max-width: 768px)
    padding-bottom: 0
  ::v-deep(.main-title)
    justify-content: flex-end
    gap: 96px
    margin-top: -.5em
    @media screen and (max-width: 768px)
      font-size: 20px
      gap: 32px
  .logos
    width: 100%
    white-space: nowrap

.call-for-paper
  margin: 7vh 0
  margin-left: auto
  padding: .5em 2em
  width: 10em
  color: #32e0c4
  font-weight: 900
  text-align: center
  display: block
  position: relative
  line-height: 1
  @media screen and (max-width: 768px)
    padding: .5em 1em
    padding-right: 1em
    width: 9em
  .corner
    position: absolute
    height: .7em
    width: .7em
    background-image: url(/imgs/cfp/corner.svg)
    background-size: contain
    background-repeat: no-repeat
    &:nth-child(1)
      top: -10px
      left: -10px
    &:nth-child(2)
      top: -10px
      right: -10px
      transform: rotate(90deg)
    &:nth-child(3)
      bottom: -10px
      left: -10px
      transform: rotate(270deg)
    &:nth-child(4)
      bottom: -10px
      right: -10px
      transform: rotate(180deg)

.round-btns
  width: 100%
  display: grid
  grid-row: 1
  direction: rtl
  grid-row-gap: 20px
  @media screen and (max-width: 768px)
    grid-row-gap: 15px

.prev-sites
  display: grid
  grid-template-columns: repeat(4,1fr)
  gap: 24px
  @media screen and (max-width: 768px)
    grid-template-columns: repeat(2,1fr)

.rad-btns
  display: flex
  gap: 24px
  align-items: flex-start
  margin-top: 36px
  @media screen and (max-width: 768px)
    margin: 16px 0
    gap: 12px
    flex-direction: column

.cat-background
  @media screen and (min-width: 960px)
    position: relative
    &:before
      content: ''
      position: absolute
      bottom: 20px
      right: 100px
      width: 212px
      height: 212px
      background-image: url(/imgs/cfp/cat.png)
      background-repeat: no-repeat
      background-size: contain
      background-position: bottom right
      animation: floating-cat-animation 10s ease-in-out infinite

@keyframes floating-cat-animation
  from
    transform: translateY(0px)
  65%
    transform: translateY(-20px)
  to
    transform: translateY(0px)

.margin-0
  margin: 0

.cfp-glass-box
  border-radius: 25px
</style>
