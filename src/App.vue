<template>
    <div class="page-view">
        <div class="page-content">
            <div class="layout">
                <div class="topnav">
                    <!-- <router-link to="/about-us">
                        {{topInfo.name}}
                    </router-link> -->
                    <div v-for="item in advList" class='topAd' >
                        <div @click="noticedeail(item.id)">{{item.title}}
                        </div>
                    </div>
                </div>
                <div class="layout-ceiling">
                    <router-link to="/">
                        <div class="layout-logo"></div>
                    </router-link>
                    <div class="layout-ceiling-main">
                        <div class="header_nav">
                            <Menu :active-name="activeNav" width="auto" :open-names="['1']">
                                <Submenu name="1">
                                    <router-link to="/">
                                        <MenuItem name="nav-index">{{$t("header.index")}}</MenuItem>
                                    </router-link>
                                    <router-link to="/otc/trade/btc">
                                        <MenuItem name="nav-otc">{{$t("header.otc")}}</MenuItem>
                                    </router-link>
                                     <router-link to="/exchange">
                                        <MenuItem name="nav-exchange">{{$t("header.exchange")}}</MenuItem>
                                    </router-link>
                                    <router-link to="/finance">
                                        <MenuItem name="nav-asset">{{$t("header.asset")}}</MenuItem>
                                    </router-link>
                                    <router-link to="/uc/safe">
                                        <MenuItem name="nav-uc">{{$t("header.ucenter")}}</MenuItem>
                                    </router-link>
                                    <router-link to="/help">
                                        <MenuItem name="nav-service">{{$t("header.service")}}</MenuItem>
                                    </router-link>
                                </Submenu>
                            </Menu>
                        </div>
                        <div class="rr">
                            <div class="login_register" v-if="isLogin">
                                <Dropdown>
                                    <a href="javascript:void(0)">
                                        <Icon type="person" style="font-size: 20px;vertical-align: middle;"></Icon>
                                        <span>{{member.username}}</span>
                                        <Icon type="arrow-down-b"></Icon>
                                    </a>
                                    <DropdownMenu slot="list">
                                        <div @click="logout">
                                            <DropdownItem>
                                                <img src="./assets/images/logout.png"> {{$t("common.logout")}}
                                            </DropdownItem>
                                        </div>
                                    </DropdownMenu>
                                </Dropdown>
                            </div>
                            <div class="login_register" v-else>
                                <Menu active-name11="1-1"  width="auto" :open-names="['2']">
                                    <Submenu name="2">
                                        <router-link to="/login" id="login">
                                            <MenuItem name="1-1">{{$t("common.login")}}</MenuItem>
                                        </router-link>
                                        <router-link to="/register" id="register">
                                            <MenuItem name="1-2">{{$t("common.register")}}</MenuItem>
                                        </router-link>
                                    </Submenu>
                                </Menu>
                            </div>

                            <Dropdown @on-click="changelanguage">
                                <a style="width:90px;height:20px;line-height:20px;border:1px solid;border-radius:20px;padding:0 12px;" href="javascript:void(0)">
                                    {{languageValue}}
                                    <Icon type="arrow-down-b"></Icon>
                                </a>
                                <DropdownMenu slot="list">
                                    <DropdownItem v-if="languageValue=='繁体中文'" name="en">English</DropdownItem>
                                    <DropdownItem v-else name="cn">繁体中文</DropdownItem>
                                    <!--<DropdownItem name="hk">繁体中文</DropdownItem>-->
                                </DropdownMenu>
                            </Dropdown>
                        </div>
                    </div>
                </div>
            </div>
            <router-view></router-view>
            <div class="footer">
                <div class="footer_content">
                    <div class="footer_left">
                        <!--<img src="./assets/images/footer_logo.png"></img>-->
                        <!-- <h3>weilan.Pro</h3> -->
                        <p>{{$t("footer.gsmc")}}</p>
                        <p>Copyright © 2017 - 2018&nbsp;&nbsp;</p>
                    </div>
                    <div class="footer_right">
                        <ul>
                            <li class="footer_title">
                                <span>{{$t("footer.gsjj")}}</span>
                            </li>
                            <li>
                                <router-link to="/about-us">{{$t("footer.gywm")}}</router-link>
                            </li>
                            <li>
                                <router-link to="/join-us">{{$t("footer.jrwm")}}</router-link>
                            </li>
                        </ul>
                        <ul>
                            <li class="footer_title">
                                <span>{{$t("footer.bzzx")}}</span>
                            </li>
                            <!-- <li>
                               
                              <router-link to="/newhelp/index?id=3">{{$t("cms.faq")}}</router-link>
                            </li> -->
                            <li>
                                <!--<a href="#">{{$t("footer.xsrm")}}</a>-->
                              <router-link to="/newhelp/index?id=0">{{$t("footer.xsrm")}}</router-link>
                            </li>
                            <li>
                                <!--<a href="#">{{$t("footer.czzn")}}</a>-->
                              <router-link to="/newhelp/index?id=1">{{$t("footer.czzn")}}</router-link>
                            </li>
                            <li>
                                <!--<a href="#">{{$t("footer.jyzn")}}</a>-->
                              <router-link to="/newhelp/index?id=2">{{$t("footer.jyzn")}}</router-link>
                            </li>
                        </ul>
                        <ul>
                            <li class="footer_title">
                                <span>{{$t("footer.ptsm")}}</span>
                            </li>
                            <li>
                                <router-link to="/about-rule">{{$t("footer.fysm")}}</router-link>
                            </li>
                            <li>
                                <router-link to="/about-protocol">{{$t("footer.fwtk")}}</router-link>
                            </li>
                            <li>
                                <router-link to="/about-fee">{{$t("footer.fltk")}}</router-link>
                            </li>
                        </ul>
                        <ul>
                            <li class="footer_title friendlink">
                                <span>{{$t("footer.lxwm")}}</span>
                            </li>
                             <li>
                                <div class="bdshare">
                                    <a href="https://www.facebook.com/blockchain.blockchain.944" target="_blank"><img src="./assets/images/facebook.png" alt=""></a>
                                    <a href="https://twitter.com/BlockchainGrou4" target="_blank"><img src="./assets/images/foot_bried.png" alt=""></a>
                                    <a href="https://www.linkedin.com/in/blockchain-group-95889b163/" target="_blank"><img src="./assets/images/foot_in.png" alt=""></a>
                                    <a href="https://www.instagram.com/blockchaingroup_official/" target="_blank"><img src="./assets/images/foot_instagram.png" alt=""></a>
                                    <a href="https://www.youtube.com/channel/UCjYzcf3mNS8jYhDvhETor-w?view_as=subscriber" target="_blank"><img src="./assets/images/foot_youtube2.png" alt=""></a>
                                    <a href="https://t.me/joinchat/GHdVcU7SajdIsEdTY3GVjw" target="_blank"><img src="./assets/images/foot_tele.png" target="_blank" alt="" ></a>    
                                    <!-- <a href="#" class="bds_fbook" data-cmd="fbook" title="分享到Facebook"></a>
                                    <a href="#" class="bds_twi" data-cmd="twi" title="分享到Twitter"></a> -->
                                </div>

                            </li>
                            <!-- <li>
                                <a href="javascript:;">kefu@weilan.pro</a>
                            </li>
                            <li>
                                <a href="https://0.plus/Caymanofficial" target="_blank">币用</a><a href="http://t.me/Caymanofficial" target="_blank">telegram</a>
                            </li> -->
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import Vue from 'vue';
import { mapGetters, mapActions } from 'vuex';
export default {
    name: 'app',
    data() {
        return {
            // topInfo:{name:'weilan--领衔全球的数字资产交易平台',remark:'aaaa',createTime:'2018-01-10 11:37:27'}
            // languageValue: '简体中文'
            advList:[],
        }
    },
    watch:{
      'activeNav':function () {
        switch (this.activeNav) {
          case "nav-exchange":
            break;
          default:
            window.document.title="BlockChain Exchange";
            break;
        }
      }
    },
    computed: {
        'activeNav': function() {
            return this.$store.state.activeNav;
        },
        'isLogin': function() {
            return this.$store.getters.isLogin;
        },
        'member':function(){
            return this.$store.getters.member;
        },
        'languageValue':function () {
            var curlang = this.$store.getters.lang;
            console.log(curlang)
            if(curlang == "English") this.$i18n.locale = 'en';
            if(curlang != "English") this.$i18n.locale = 'zh';
            return curlang;
        }
    },
    created: function() {
        if (this.isMobileUserAgent()){
        //   location.href = "https://wap.caymanex.pro/";
          return;
        }
        var that = this;
        if ('-ms-scroll-limit' in document.documentElement.style && '-ms-ime-align' in document.documentElement.style) { // detect it's IE11
		  window.addEventListener("hashchange", function(event) {
		    var currentPath = window.location.hash.slice(1);
		    if (that.$router.path !== currentPath) {
		      that.$router.push(currentPath)
		    }
		  }, false)
		}
        this.initialize();
        this.loadDataPage(1)
    },
    methods: {
        isMobileUserAgent:function(){
          return (/iphone|ipod|android|windows.*phone|blackberry.*mobile/i.test(window.navigator.userAgent.toLowerCase()));
        },
        initialize() {
            this.$store.commit('navigate','nav-index');
            this.$store.commit('recoveryMember');
            this.$store.commit('initLang');

            // this.loadTopInfo();
            this.checkLogin();
        },
        loadTopInfo(){ /*获取首页顶部公告*/
          let param = {};
          param["sysAdvertiseLocation"] = 2;
          this.$http.post(this.host + '/uc/ancillary/system/advertise', param).then(response => {
            var result = response.body;
            if(result.code == 0 && result.data.length > 0){
              this.topInfo = result.data[0];
            }
          });
        },
        logout() {
            this.$http.post(this.host + '/uc/logout', {}).then(response => {
                var resp = response.body;
                if (resp.code == 0) {
                    this.$Message.success(resp.message);
                    this.$store.commit('setMember',null);
                    location.href = "/";
                } else {
                    this.$Message.error(resp.message);
                }
            })
        },
        checkLogin() {
            this.$http.post(this.host + '/uc/check/login', {}).then(response => {
                var result = response.body;
                if(result.code == 0 && result.data == false){
                   this.$store.commit('setMember',null);
                }
            });
        },
        changelanguage: function(name) {
            if (name == 'en') {
                // this.languageValue = 'English';
                this.$store.commit('setlang','English');
                this.$i18n.locale = 'en';
            }
            if (name == 'cn') {
                // this.languageValue = '繁体中文';
                this.$store.commit('setlang','繁体中文');
                this.$i18n.locale = 'zh';
            }
            // if (name == 'hk') {
            //      this.languageValue = '繁体中文';
            // }
        },
        // 顶部公告
        loadDataPage(pageIndex){
            var param = {};
            param["pageNo"] = pageIndex,
            param["pageSize"] = 1,
            this.$http.post(this.host + this.api.uc.announcement, param).then(response => {
                var resp = response.body.data.content;
                this.advList=resp;
           
            })
        },
        // 公告跳转
        noticedeail(x){
            this.$router.push({ path:'/notice/index', query:{id:x}});
        }
    }
}
</script>

<style>
/* 帮助中心 */
.article .content span p{
    margin-right:0 !important;
    margin-left: 0 !important;
}

/* 模态框 */
.ivu-modal-confirm-body{
    color:#A69C8C;
}
.ivu-modal-wrap{
    background-color:rgba(0,0,0,.5);
}
.ivu-modal-content{
    background-color:#3D3E42;
}
.ivu-modal-header p, .ivu-modal-header-inner{
    color:#D58C2A;
}
.ivu-modal-footer button+button{
    background-color: #999081;
    color: #3E3F42;
}
.ivu-modal-wrap .ivu-btn-primary:hover{
    background-color: #999081;
    color: #3E3F42;
}
.ivu-modal-header,.ivu-modal-body{
    border-bottom:1px  solid  #54514A;
}
.ivu-modal-footer{
    border-top:1px  solid  #54514A;
}
.ivu-upload-drag{
    background-color:transparent;
}

/* 页码 */
.ivu-page-item-active{
    background-color:transparent;
    border-color: #413F40;
}
.ivu-page-next, .ivu-page-prev{
    background-color: #413F40;
    border-color: #413F40;
    color:#E6D7C3;
}
/* 按钮 */
.ivu-btn-success{
    background-color:#37F081;
    border-color:#37F081;
    color:#fff;
}
/* 财务中心 */
.order-table .ivu-btn-primary{
    background-color:#37F081;
    border-color:#37F081;
    color:#fff;
}
.order-table .ivu-btn-error{
    background-color:#F35339;
    border-color:#F35339;
    color:#fff; 
}

.ivu-tabs-bar{
    border-color:#828387;
}
.ivu-menu-light{
    background-color:#232328;
}
.ivu-menu-vertical.ivu-menu-light:after{
    background:transparent;
}
a{
    color:#D58C2A;
}
/* 表格头部切换 */
.ivu-tabs-nav .ivu-tabs-tab{
    color: #9A9083
}
.ivu-tabs-nav .ivu-tabs-tab-active,.ivu-tabs-nav .ivu-tabs-tab:hover{
    color:#D58C2A;
}
.ivu-tabs-nav-container:focus .ivu-tabs-tab-focused{
    border-color:#D58C2A !important;
}

.bdselect_share_bg{
    z-index:-1 !important;
}
.ivu-table{
    color:#A69C8C;
}
.ivu-table-wrapper{
    border-top:1px solid transparent;
}
/* .ivu-btn-info{
    background-color:#D58C2A;
    border-color:#D58C2A;
} */

.ivu-carousel-dots-inside{
    bottom:9px;
}
.content100 .ivu-poptip-rel{
    width:100%;
}
.ivu-menu-light.ivu-menu-vertical .ivu-menu-item-active:not(.ivu-menu-submenu){
    color:#9D9286;
}
.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item{
    color:#675D54;
}
.ivu-select-dropdown{
    background-color:#323031;
}
.ivu-select-selection{
    border-color:#323031 !important;
}
.ivu-select-selection,.ivu-input-number-input,.ivu-input-number,.ivu-input-number-input[disabled]:hover{
     background-color:transparent;
}
.ivu-select-visible .ivu-select-selection{
    border-color:#323031;
}
.ivu-input[disabled], fieldset[disabled] .ivu-input{
    background-color:#323031;
}
.ivu-input-group-append, .ivu-input-group-prepend{
    background-color:transparent;
    color:#A69C8C;
    border-color: #323031;
}
.ivu-switch{
    background-color:transparent;
}
.ivu-switch-checked,.ivu-checkbox-checked .ivu-checkbox-inner{
    background-color:#D58C2A;
    color:#D58C2A;
    border-color:#D58C2A;
}
.ivu-alert-info{
    border: 1px solid #323031;
    background-color: #323031;
    color:#9A9083;
}
.ivu-tabs-ink-bar{
    background-color:#D58C2A;
}
.ivu-table-wrapper{
    border:none;
}

.ivu-select-single .ivu-select-selection .ivu-select-placeholder, .ivu-select-single .ivu-select-selection .ivu-select-selected-value{
    color:#9D9286;
}
/* 禁止点击 */
.ivu-input-number-disabled .ivu-input-number-input{
    background-color: #323031;
}
.ivu-btn,.ivu-btn-ghost:hover{
    border-color:transparent;
    color:#9A9083;
}
/* 顶部公告 */
.topAd {
    text-align:center;
    padding:10px 0;
}
.topAd div{
    display:inline-block;
    color:#9A9083;
    font-size:16px;
    cursor: pointer;
}

li{
    list-style:none;
}

  #onlineservice{
    position: fixed;
    right: 20px;
    bottom: 40px;
    background: transparent;
}
  #onlineservice>a{
    background: transparent url("assets/images/onlineservice.jpg") no-repeat;
    display: block;
    /*width: 80px;*/
    /*height: 80px;*/
    width: 64px;
    height: 66px;
    background-size: cover;
    /*border-radius: 100%;*/
  }

/* top */
.ivu-select-selection .ivu-select-selected-value {
    color: #9D9286;
}
.topnav {
    text-align: center;
    line-height: 25px;
    background: #191c23;
}

.topnav a {
    color: #fff;
    font-size: 14px;
}

/*  */
.ivu-menu-light.ivu-menu-vertical .ivu-menu-item{
    border-color:#222327;
    color:#9A9083;
}
.ivu-menu-light.ivu-menu-vertical .ivu-menu-item-active:not(.ivu-menu-submenu) {
    border-right: none;
  
}
#List .ivu-col-span-4 .ivu-menu-light.ivu-menu-vertical .ivu-menu-item-active:not(.ivu-menu-submenu){
      background-color:#323031;
}

.header_nav .ivu-menu-vertical.ivu-menu-light:after {
    width: 0;
}

.header_nav .ivu-menu-vertical .ivu-menu-item:hover,
.ivu-menu-vertical .ivu-menu-submenu-title:hover {
    background: none;
    color: #D58C2A ;
}
/*  */

html,
body {
    height: 100%;
    margin: 0;
    padding: 0;
    background: #191c23;
    color:#A69C8C;
    font-family: "Helvetica Neue", Helvetica, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑", Arial, sans-serif;
}

/*自定义滚动条样式*/

::-webkit-scrollbar {
    width: 10px;
    background: #eee;
}

::-webkit-scrollbar-thumb {
    background: #eee;
    border-radius: 25px;
}

.hide {
    display: none;
}

.blue {
    color: #6BF !important;
}

.red {
    color: #AE4E54 !important;
}





.ivu-table-header{
    background-color:#323031;
    color:#9A9083;
}

.ivu-table:after,.ivu-table:before{
    background-color:transparent;
}
.ivu-table-body{
    color:#9A9083;
}
.ivu-input{
    background:transparent;
    border:1px solid #323031;
    color:#9D9286;
}
.ptjy .ivu-table,.ptjy .ivu-table td{
    border-bottom:1px solid #191c23 !important;
    color:#E3E3E3;
}
.ivu-table,.ivu-table td{
    background:transparent !important; 
}
.ivu-table th{
    background-color:#323031;
    color:#9A9083;
}
.ivu-table td, .ivu-table th{
    border-bottom:1px solid #828387 !important;
}
.ivu-btn-info,.ivu-btn-info:hover {
    background:#999081;
    border-color:#9A9083;
    color:#303231;
}

.ivu-btn-primary {
    background:#999081;
    border-color:#9A9083;
    color:#303231;
}

.ivu-btn.active,
.ivu-btn:active {
    color:#D58C2A;
    background: #323031;
    border-color: #323031;
}
.login_right .ivu-btn{
    background-color:transparent;
    border-color:#323031;
}
.login_right .ivu-btn.active,.login_right  .ivu-btn:active{
    color:#D58C2A;
    background: #323031;
    border-color: #323031;
}
.login_right .ivu-btn:hover{
    color:#D58C2A;
}
.login_right .ivu-form-item-content .ivu-btn-info{
    background-color:#413F40;
    color:#D58C2A;

}
.ivu-btn-text.active,
.ivu-btn-text:active {
    color: #2b85e4;
    background-color: transparent;
    border-color: transparent;
}

.ivu-btn.disabled,
.ivu-btn.disabled.active,
.ivu-btn.disabled:active,
.ivu-btn.disabled:focus,
.ivu-btn.disabled:hover,
.ivu-btn[disabled],
.ivu-btn[disabled].active,
.ivu-btn[disabled]:active,
.ivu-btn[disabled]:focus,
.ivu-btn[disabled]:hover,
fieldset[disabled] .ivu-btn,
fieldset[disabled] .ivu-btn.active,
fieldset[disabled] .ivu-btn:active,
fieldset[disabled] .ivu-btn:focus,
fieldset[disabled] .ivu-btn:hover {
    color: #fff;
    background: #54677F;
}

.ivu-carousel-dots li button {
    width: 30px;
    height: 10px;
    border-radius: 14px;
}

.ivu-menu-dark,
.ivu-menu-dark.ivu-menu-vertical .ivu-menu-opened {
    background: #18202A;
}

#checkbox {
    width: 10px;
}

#sendCode {
    position: absolute;
    border: 0;
    top: 0;
    right: 0;
    width: 30%;
    background-color:#D58C2A;
    color:#fff;
    cursor: pointer;
}

.login_form {
    background: url(./assets/img/carousel.png) no-repeat center;
    height: 760px;
    background-size: cover;
    position: relative;
    overflow: hidden;
}

.login_left {
    width: 46%;
    height: 400px;
    margin: 7% auto;
    background: rgba(0,0,0,.4);
    position: relative;
    padding: 0 50px;
    color: #979797;
    font-size: 20px;
    margin-right: 4%;
}

.login_right {
    position: absolute;
    background: #222327;
    width: 350px;
    height: 510px;
    top: -55px;
    right: 0;
}

.login_title {
    color: #D58C2A;
    text-align: center;
    height: 80px;
    font-size: 25px;
}

/* 极验证 */
.geetest_holder.geetest_wind .geetest_radar_tip, .geetest_holder.geetest_wind .geetest_success_radar_tip{
    background-color:#413F40;
    color:#D58C2A !important;
}
.geetest_holder.geetest_wind .geetest_radar_btn, .geetest_holder.geetest_wind .geetest_success_btn{
    border:1px solid #413F40 !important;
}






/* .login_right .ivu-select-selection{
        background:#EAEDEE;
} */

.login_right .ivu-select-dropdown {
    /* background: #fff; */
}

.ivu-form-inline .ivu-form-item {
    display: block;
    margin-right: 0;
}









/* .user_center{
    padding:20px 10%;
}
.user_center .ivu-select-selection,.user_center .ivu-input{
    background:#263142;
    border:0;
    color:#fff;
}
.user_center .ivu-select-dropdown{
    background:#263142;
    color:#fff;
}
.user_center .ivu-select-item{
    color:#fff;
}
.user_center .ivu-select{
    color:#fff;
}
.user_center .ivu-select-item:hover,.user_center .ivu-select-item-selected,.user_center .ivu-select-item-selected:hover{
    background:#495060;
}
.user_center .ivu-table th{
        text-align:center;
        background:#28313E;
        color:#979797;
        border:0;
}
.user_center .ivu-table td{
        background:none;
        text-align:center;
        border-bottom:2px dashed #263142;
} */

.modify .ivu-input-wrapper {
    width: 40%;
}

.ivu-btn-ghost {
    /* color:#fff; */
}

.layout {
    position: relative;
    background-color:#222327;
}

.layout-logo {
    width: 86px;
    height: 51px;
    background: url(./assets/images/logo.png) no-repeat;
    background-size:contain;
    float: left;
    position: relative;
}

.layout-copy {
    text-align: center;
    padding: 10px 0 20px;
    color: #9ea7b4;
}

.layout-ceiling {
    padding: 15px 10px;
    overflow: hidden;
    max-width:1310px;
    min-width:1180px;
    width:100%;
    margin:0 auto;
}

.layout-ceiling-main {
    /* float: left; */
    height: 50px;
    line-height: 50px;
    margin-left: 150px;
}

.layout-ceiling-main .rr {
    float: right;
}

.layout-ceiling-main .ivu-menu-vertical .ivu-menu-item,
.ivu-menu-vertical .ivu-menu-submenu-title {
    padding: 0;
}

.layout-ceiling-main .ivu-menu-item {
    font-size: 14px;
}

.layout-ceiling-main a {
    color: #9A9083;
    display: inline-block;
    line-height: 40px;
    height: 40px;
    text-align: center;
    margin-left: 30px;
    /*padding: 0 15px;*/
}

.header_nav {
    float: left;
    margin-right: 20px;
}

.header_nav .ivu-menu-dark.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item-active,
.header_nav .ivu-menu-dark.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item-active:hover {
    background: url(./assets/images/menu_active.png) !important;
}

.login_register .ivu-menu-dark.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item-active,
.login_register .ivu-menu-dark.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item-active:hover {
    background: #1855fd;
    border-radius: 5px;
}

.login_register {
    float: left;
}

#login.router-link-active,
#register.router-link-active{
    background: #323031;
    color:#9A9083;
    border-radius: 5px;
}
/* #login.router-link-active li,
#register.router-link-active li{
    color:#fff;
} */
#login,
#register {
    color: #fff;
    display: inline-block;
    line-height: 25px;
    width: 75px;
    height: 25px;
    text-align: center;
    margin: 0;
}

.login_register a {
    margin-left: 0;
}

.ivu-dropdown-rel a {
    width: 100%;
}

.ivu-dropdown-menu {
    width: 100px;
}

.layout-ceiling-main .ivu-select-dropdown {
    background: #0b0d1b;
    margin-left: 25px;
}

.ivu-select-dropdown a {
    width: 100%;
    text-align: left;
    margin: 0;
}

.ivu-dropdown-item:hover {
    background: #aaa;
}

.ivu-dropdown-item {
    color: #fff;
}

.ivu-dropdown-item img {
    vertical-align: middle;
}

.ivu-radio-inner:after {
    background: #18202A;
}









/*安全中心*/

.user_center {
    height: 900px;
}

.ivu-menu-submenu-title {
    display: none;
}

.ivu-menu-item {
    text-align: center;
}

.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item {
    padding-left: 0 !important;
    padding-right: 0;
    color: #675D54;
    font-size: 16px;
    border-right: 0 !important;
}

.ivu-menu-dark.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item-active,
.ivu-menu-dark.ivu-menu-vertical .ivu-menu-submenu .ivu-menu-item-active:hover {
    background: #1855fd !important;

}

.rr .ivu-menu-vertical .ivu-menu-item:hover,
.ivu-menu-vertical .ivu-menu-submenu-title:hover {
    background: none;
    color: #D58C2A ;
    
}

.rr .ivu-menu-vertical.ivu-menu-light:after {
    width: 0;
}

.layout_menu_right {
    margin-left: 3%;
    background: #18202A;
    color: #fff;
    padding-bottom: 130px;
}

.menu_right_title {
    font-size: 16px;
    line-height: 45px;
    margin: 0 10px;
    padding-left: 20px;
    border-bottom: 1px solid #263142;
}



 .ivu-form .ivu-form-item-label{
        color:#9F9686;
    }
 /*   .ivu-form-item-required .ivu-form-item-label:before{
        display:none;
    } */

.category .ivu-radio-group.ivu-radio-group-button {
    width: 100%;
}

.category .ivu-radio-group label {
    font-size: 14px;
}

.category .ivu-radio-group-button .ivu-radio-wrapper {
    background: #28313E;
    color: #979797;
    border: 0;
    padding: 0 25px;
}

.category .ivu-radio-group-button .ivu-radio-wrapper-checked {
    color: #fff;
    background: #2F3D52;
    box-shadow: none;
}

.category .ivu-radio-wrapper span {
    padding-left: 0;
}

.purse_address_left {
    float: left;
    width: 86%;
}

.purse_address p {
    font-size: 10px;
    line-height: 25px;
    color: #979797;
}

.purse_address_left_icon {
    line-height: 40px;
    height: 40px;
    width: 100%;
}

.purse_address_left_icon img {
    vertical-align: middle;
    margin-right: 10px;
}

.purse_address span {
    font-size: 14px;
    float: left;
    color: #fff;
    padding: 0 20px;
    background: #28313E;
    width: 21%;
}

.purse_address_left_icon label {
    float: left;
    width: 72%;
    height: 40px;
    border: 2px solid #28313E;
    padding-left: 20px;
}

#qrcode canvas {
    width: 120px;
}

#qrcode img {
    width: 100%;
}
.ivu-select-item{
    color:#9D9286;
}
.ivu-select-item:hover {
    background: #323031;
}

.ivu-select-item-selected,
.ivu-select-item-selected:hover {
     background:rgba(0,0,0,.1)
}
.ivu-select-item-selected.ivu-select-item-focus{
     background:rgba(0,0,0,.1)
}

.chart_container #chart_updated_time {
    float: left;
}

.footer {
    float: left;
    width: 100%;
}

.footer_content {
    height: 200px;
    padding: 50px 10%;
    color: #53575c;
    color:rgba(255,255,255,.8);
    background: #222327;
}

.footer_left {
    float: left;
    font-size: 14px;
}

.footer_left img {
    margin: 15px 0;
}

.footer_left p {
    margin: 10px 0;
    color:#9A9083;
}

.footer_right {
    float: right;
    /*margin-top: 15px;*/
    text-align: center;
    /* margin-right: 20px; */
}

.footer_right ul {
    float: left;
    margin: 0 30px;
}
.footer_right ul li{
    color:#9A9083;
}
.footer_right ul li a {
    color:#665F57;
    line-height: 25px;
    display: block;
}

.footer_title {
    font-size: 15px;
    height: 35px;
    text-align:text;
    color:#9A9083;
}
.footer_title.friendlink{
    text-align: left;
}
.ivu-select-selected-value {
    color: #bbbec4
}

/*法币交易*/

.ivu-col {
    text-align: center;
}

/* 账户中心的验证码 */
.googel .qrCode,.googel .secretKey{
    display:inline-block;
    vertical-align:middle;
    margin-right:20px;
    text-align:left;
}
/* 协议 */
.agreement .content{
    width:80%;
    min-width:1200px;
    margin:0 auto;
}

/* 表格样式 */
.ivu-table td, .ivu-table th{
    text-align:center;
}
.order-table .ivu-table-body table,.order-table .ivu-table-header table{
    width:auto !important;
}
.order-table .ivu-table-header table th,.order-table .ivu-table-body table td{
    width:120px;
}

/* 百度分享 */

.footer  a.bds_tsina{
    background:url(./assets/img/i1.png);
}
.footer  a.bds_weixin{
    background:url(./assets/img/i2.png);
}
.footer  a.bds_fbook{
    background:url(./assets/img/i3.png);
}
.footer  a.bds_twi{
    background:url(./assets/img/i4.png);
}
.footer .bdshare  a{
    height:24px;
    padding-left:0px;
}
.footer .bdshare {
    display: flex;
    width: 200px;
    justify-content: space-between;
}
.bdselect_share_box{
    z-index:-1 !important;
}
.sr-bdimgshare {
    z-index:-1 !important;
}
#bdshare_weixin_qrcode_dialog{
    height:314px !important;
}

/* 上传图片 */
.ivu-upload .ivu-upload-list .ivu-upload-list-file-finish{
    display:none;
}
</style>
