<template>
    <div class="content-wrap finance_list" >
            <div class="container" id="List" style='min-height:700px;margin-bottom:20px;background-color:#222327;'>
                <Row>
                    <Col span="4">
                    <div class="leftmenu">
                        <ul class="nav nav-pills nav-stacked finance_list_ul">
                            <span class="leftmenu-title leftmenu-folding top" data-folding="trademenu1">
                                <!-- <i class="lefticon icon4"></i> -->
                                {{$t('uc.finance.center')}}
                            </span>
                            <li class="">
                                <!-- <router-link to="/finance/index"> -->

                                <i-button @click="instance('warning')" style="background-color: rgb(34, 35, 39);width:100%;">{{$t('uc.finance.personalassets')}}</i-button>
                                <!-- </router-link> -->
                            </li>
                            <li class="">
                                <!-- <router-link to="/finance/record">  -->
                                <i-button  @click="instance('warning')" style="background-color: rgb(34, 35, 39);width:100%;">{{$t('uc.finance.billdetail')}}</i-button>
                                <!-- </router-link> -->
                                
                            </li>
                            <!-- <span class="leftmenu-title leftmenu-folding " data-folding="trademenu2">
                                <i class="lefticon icon5"></i>
                                充值提现
                            </span> -->
                            <li class="">
                                <!-- <router-link to="/finance/recharge"> -->
                                 <i-button  @click="instance('warning')"  style="background-color: rgb(34, 35, 39);width:100%;">{{$t('uc.finance.charge')}}</i-button>
                                <!-- </router-link> -->
                            </li>
                            <li class="">
                                <!-- <router-link to="/finance/withdraw"> -->
                                 <i-button  @click="instance('warning')" style="background-color: rgb(34, 35, 39);width:100%;" >{{$t('uc.finance.pickup')}}</i-button>
                                <!-- </router-link> -->
                            </li>
                        </ul>
                    </div>
                    </Col>
                    <Col span="20" >
                    <!-- <keep-alive> -->
                    <router-view></router-view>
                    <!-- </keep-alive> -->
                    </Col>
                </Row>
            </div>
    </div>
</template>
<script>
export default {
    components: {
    },
    data() {
        return {

        }
    },
    methods: {
        init() {
            this.$store.commit('navigate','nav-asset');
            this.$store.state.HeaderActiveName = '1-5';
            if (!localStorage.TOKEN || !localStorage.MEMBER) {
                this.$Message.error(this.$t('common.logintip'));
                this.$router.push('/login');
            }
        },
        instance (type) {
                const title = '';
                const content = '<p>Functionality coming up</p>';
                switch (type) {
                    case 'warning':
                        this.$Modal.warning({
                            title: title,
                            content: content,
                            okText:'sure',
                        });
                        break;
                }
            }
        
    },
    created: function() {
        this.init();
    },
}
</script>
<style>
.finance_list .ivu-btn:hover{
    background-color:rgb(34, 35, 39) !important;
    border-color:rgb(34, 35, 39);
    color:#9D9286;
}
.finance_list .ivu-btn:focus{
    box-shadow:0 0 0 0!important;
}
/* .ivu-modal-confirm-body p{
    font-size: 20px !important;
} */
</style>

<style scoped>



.leftmenu a.router-link-active {
    background-color: #323031;
    color: #9D9286;
}

.icon4 {
    background: url('../../assets/img/moneyicon1.png') no-repeat 0 0;
    background-size: 100% 100%;
}

.icon5 {
    background: url('../../assets/img/moneyicon2.png') no-repeat 0 0;
    background-size: 100% 100%;
}

.order-table {
    margin-top: 20px;
}

.content-wrap {
    background: #191c23;
    min-height: 450px;
    padding-top:20px;
}

.container {
    width: 80%;
    margin: 0 auto;
    min-width: 1200px;
    /* background:white; */
    padding-top: 30px;
}



/* left */

.leftmenu {
    margin-bottom: 60px;
    /* background: #fff; */
    position: relative;
    min-height: 1px;
    padding: 20px 0;
}

.nav {
    margin-bottom: 0;
    padding-left: 0;
    list-style: none;
}

.nav>li {
    line-height: 50px;
}

.leftmenu .nav-stacked {
    /* background: #fff; */
}

.leftmenu .leftmenu-title {
    line-height: 55px;
    font-size: 20px;
    background: 0 0;
    color: #0B0D1B;
    /* padding-left: 20px; */
    /*border-top: #f1f1f1 solid 1px;
	border-bottom: #f1f1f1 solid 1px;*/
    display: block;
    /* cursor: pointer; */
}

.leftmenu .nav>li>a {
    display: block;
    color: #9D9286;
    font-size: 14px;
}

.leftmenu .nav-pills>li.active>a,
.leftmenu .nav>li>a:hover,
.nav-pills>li.active>a:focus,
.nav-pills>li.active>a:hover {
    background:#323031 ;
    color: #B9AC9E ;
}

.leftmenu .leftmenu-title.top {
    border-top: 0;
    color:#D58C2A;
}

.leftmenu .lefticon {
    width: 26px;
    height: 26px;
    margin-right: 5px;
    display: inline-block;
    vertical-align: middle;
}
</style>

