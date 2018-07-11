<template>
  <div class="container">
    <img src="../../assets/images/call.png">
    <div class="content-wrap">
      <Row>
        <Col span="4">
        <div class="leftmenu">
          <ul class="nav">
            <li class="divider">{{$t('cms.about')}}</li>
            <li class="cur">
              <router-link to="/about-us">{{$t('cms.aboutus')}}</router-link>
            </li>
            <li>
              <router-link to="/join-us">{{$t('cms.joinus')}}</router-link>
            </li>
          </ul>
        </div>
        </Col>
        <Col span="20" class="content">

          <div class=WordSection1 style='layout-grid:15.6pt' v-if="lang != 'English'">

          <p class=MsoNormal align=left style='text-align:left'><b><span lang=EN-US
                                                                         style='font-family:宋体'>&nbsp;</span></b></p>

          <p class=MsoNormal align=left style='text-align:left'>DBEX是領銜全球的數字資產交易平臺，向全球用戶提供專業、安全、便捷的數字資產投資交易服務，目前已在设立交易服務中心，並已開啟在马来西亚、日本、韩国、新加坡等地的布局。</p>

          <p class=MsoNormal align=left style='text-align:left'>在全球區塊連技術革命浪潮下，DBEX以推動全球金融改革為使命，致力於發現優質的區塊鏈數字資產，為個人提供更多、更優的數字資產投資機會，打造全球頂尖的數字資產交易平臺。</p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span
            style='font-family:宋体'>全球頂級安全風控體系</span></b></p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>全球首創的的數字資產研究評估體系</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>深耕數字資產服務產業，提供權威的資產分析</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>專業分布式架構和防DDOS攻擊系統</p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b>世界領先的技術優勢</b></p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>經權威認證多機互備的高速內存撮合技術，處理速度高達10萬單/秒，遠高於行業平均水平。</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>SSL、動態身份驗證等銀行級別安全技術</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>冷錢包、私鑰離線化的熱錢包等先進的技術</p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b>國際化專業運營團隊</b></p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>提供比特幣、萊特幣、以太坊等數字資產的幣幣和衍生品交易服務</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>全球多個國家和地區設立交易服務中心</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>眾多的合作夥伴為平臺提供流動性</p>
        </div>
        <!-- 英文 -->
        <div class=WordSection1 style='layout-grid:15.6pt' v-else>

          <p class=MsoNormal align=left style='text-align:left'><b><span lang=EN-US
                                                                         style='font-family:宋体'>&nbsp;</span></b></p>

          <p class=MsoNormal align=left style='text-align:left'>DBEX is a global digital asset trading platform that provides professional, secure and convenient digital asset investment trading services to users around the world. It has established a trading service center in Dubai, and has already opened the layout in Malaysia, Japan, South Korea, Singapore, etc.</p>

          <p class=MsoNormal align=left style='text-align:left'>Under the waves of global revolution of block chain technology, DBEX is committed to promoting global financial reforms by discovering high-quality block chain digital assets and providing individuals with more and better digital asset investment opportunities, building the world's top digital assets trading platform.</p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span
            style='font-family:宋体'>World's Top Security Risk Control System</span></b></p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>The world's first digital asset research and evaluation system</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>Deeply cultivating the digital asset service industry and provide authoritative asset analysis</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>Professional distributed architecture and anti-DDOS attack system</p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b>World's Leading Technological Advantages</b></p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>With an authoritative authentication and multi-machine backup, the high-speed memory matching technology has a processing speed of up to 100,000 single/second, which is far above the industry average.</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>Bank-level security technologies such as SSL and dynamic authentication</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>Advanced technologies such as cold wallets and hot wallets with private keys offline</p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b>International Professional Operation Team</b></p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span> Provide currency and derivative trading services for digital assets such as Bitcoin, Litecoin and Ethereum</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>Establish transaction service centers in many countries and regions around the world</p>

          <p class=MsoNormal align=left style='margin-left:0cm;text-align:left;
text-indent:0cm'><span lang=EN-US style='font-family:Wingdings'>l<span
            style='font:7.0pt "Times New Roman"'>&nbsp; </span></span>Numerous partners can provide liquidity to the platform</p>
        </div>

        </Col>
      </Row>
    </div>
  </div>
</template>
<script>
export default {
  computed:{
     'lang': function () {
          return this.$store.state.lang;
        }
  },
  watch:{
    'lang':function () {
          // this.updateLangData();
        }
  }
}
</script>
<style scoped>
.container {
  /* background: #fff; */
  overflow-x: hidden;
}

.content-wrap {
  padding-top: 20px;
  position: relative;
  width: 1200px;
  margin: 20px auto;
  background: #222327;
}

.leftmenu {
  /* border: 1px solid #efefef; */
}

.leftmenu .divider {
  font-size: 20px;
  padding: 5px;
  /* background: #efefef; */
  color: #d58c2a;
}

.leftmenu li {
  font-size: 14px;
  line-height: 30px;
  padding: 5px;
}

.leftmenu li a {
  color: #b9ac9e;
}
.leftmenu li.cur {
  background: #323031;
  color: #b9ac9e;
}

.leftmenu li a:hover {
  color: #d58c2a;
}

.leftmenu li.cur a {
  color: #9a9083;
}
.content {
  padding-top: 20px;
  /*padding-left: 200px;*/
  padding-bottom: 20px;
  text-align: left;
  padding-left: 20px;
}

.content .ivu-col {
  text-align: left;
}

.content p {
  text-indent: 2em;
  margin-bottom: 10px;
  font-size: 14px;
}
.content > div {
  padding-bottom: 20px;
}
.content h3 {
  font-size: 22px;
  font-weight: normal;
  margin-bottom: 20px;
}
.content h5 {
  font-size: 14px;
}
.WordSection1 span {
  color: #665f57;
  font-family: 宋体;
}
.WordSection1{
  color: #665f57;
  font-family: 宋体;
}
</style>
