<template>
  <div class="agreement">
    <img src="../../assets/images/call.png">
    <div class="agreement_tab">
      <div class="static_main">
        <router-link to="/about-rule" class="cur">{{$t('cms.exchangerule')}}</router-link>
        <router-link to="/about-protocol">{{$t('cms.useprotocol')}}</router-link>
        <router-link to="/about-fee">{{$t('cms.feenote')}}</router-link>
        <!-- <router-link to="/about-merchant">{{$t('cms.merchantprocotol')}}</router-link> -->
      </div>
    </div>
    <div class="content">

      <div class=WordSection1 style='layout-grid:15.6pt'>

        <p class=MsoNormal align=left style='text-align:left;vertical-align:middle'><b>{{$t('cms.exchangeruleList.fbbuyrule.title')}}</b></p>

        <p class=MsoNormal align=left style='text-align:left;vertical-align:middle'><span
          lang=EN-US style='font-family:微软雅黑'>1</span><span
          style=''>{{$t('cms.exchangeruleList.fbbuyrule.rule1')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>2</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule2')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>3</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule3')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>4</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule4')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>5</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule5')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>6</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule6')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>7</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule7')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>8</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule8')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>9</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.rule9')}}</span></p>

        <p><span style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbbuyrule.notice')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>&nbsp;</span></p>

        <p><strong><span style='font-size:10.5pt;font-family:微软雅黑;color: #A69C8C;'>{{$t('cms.exchangeruleList.fbsellrule.title')}}</span></strong></p>

        <p class=MsoNormal align=left style='text-align:left;vertical-align:middle'><span
          lang=EN-US style='font-family:微软雅黑'>1</span><span
          style=''>{{$t('cms.exchangeruleList.fbsellrule.rule1')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>2</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbsellrule.rule2')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>3</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbsellrule.rule3')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>4</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbsellrule.rule4')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>5</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbsellrule.rule5')}}</span></p>

        <p><span style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.fbsellrule.notice')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>&nbsp;</span></p>

        <p><strong><span style='font-size:10.5pt;font-family:微软雅黑;'></span>{{$t('cms.exchangeruleList.adrule.title')}}</strong></p>

         <p class=MsoNormal align=left style='text-align:left;vertical-align:middle'><span
          lang=EN-US style='font-family:微软雅黑'>1</span><span
          style=''>{{$t('cms.exchangeruleList.adrule.rule1')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>2</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.adrule.rule2')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>3</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.adrule.rule3')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>4</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.adrule.rule4')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>5</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.adrule.rule5')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>6</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.adrule.rule6')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>7</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.adrule.rule7')}}</span></p>

        <p><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>8</span><span
          style='font-size:10.5pt;font-family:微软雅黑;'>{{$t('cms.exchangeruleList.adrule.rule8')}}</span></p>

        <p><strong><span lang=EN-US style='font-size:10.5pt;font-family:微软雅黑;'>&nbsp;</span></strong></p>
           <p><span style='font-size:10.5pt;font-family:微软雅黑;'><b>{{$t('cms.exchangeruleList.adrule.notice')}}</b></span></p>
        <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                    style='font-family:微软雅黑'>&nbsp;</span></p>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .agreement {
    /* background: #fff; */
    padding-bottom: 20px;
    overflow-x: hidden;
  }

  .agreement_tab {
    height: 49px;
    text-align: center;
    margin-bottom: 20px;
    border-bottom: 1px solid #222327;
  }

  .agreement_tab a {
    padding: 0 4px 16px;
    margin: 0 32px;
    color: #666;
    font-size: 14px;
    line-height: 48px;
  }

  .agreement_tab a.cur {
    color: #D58C2A;
    font-weight: bold;
    border-bottom: 2px solid #D58C2A;
  }

  /*.content {*/
    /*width: 1200px;*/
    /*margin: 0 auto;*/
    /*font-size: 14px;*/
  /*}*/

  /*.content p {*/
    /*line-height: 1.5;*/
    /*margin-bottom: 10px;*/
  /*}*/

  .content{
    padding-top: 20px;
    /*padding-left: 200px;*/
    padding-bottom: 20px;
    text-align: left;
    padding-left: 20px;
    padding-right: 20px;
    background-color:#222327;
  }

  .content .ivu-col{
    text-align: left;
  }

  .content p{
    text-indent: 2em;
    margin-bottom: 10px;
    font-size: 14px;
  }
  .content>div{
    padding-bottom: 20px;
  }
  .content h3{
    font-size: 22px;
    font-weight: normal;
    margin-bottom: 20px;
  }
  .content h5 {
    font-size: 14px;
  }
  .WordSection1 span{ color:#665F57;    font-family: 宋体;}
</style>
<script>
  export default {
    components: {
    },

    computed: {
        // 'lang': function () {
        //    var lange=this.$store.state.lang;
        //    if(lange=='English'){
        //      this.$router.push('/about-ruleEn');
        //    }
        // },
       
    },
    watch:{
        'lang':function () {
           console.log(this.$store.state.lang)
        }
    },
}
</script>
