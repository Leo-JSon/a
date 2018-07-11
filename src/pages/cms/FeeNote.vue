<template>
  <div class="agreement">
    <img src="../../assets/images/call.png">
    <div class="agreement_tab">
      <div class="static_main">
        <router-link to="/about-rule">{{$t('cms.exchangerule')}}</router-link>
        <router-link to="/about-protocol">{{$t('cms.useprotocol')}}</router-link>
        <router-link to="/about-fee" class="cur">{{$t('cms.feenote')}}</router-link>
        <!-- <router-link to="/about-merchant">{{$t('cms.merchantprocotol')}}</router-link> -->
      </div>
    </div>
    <div class="content" v-if="lang=='English'?false:true">
      <div class="agreen-cont ">

        <div class=WordSection1 style='layout-grid:15.6pt'>

          <p class=MsoNormal><span lang=EN-US style='font-family:宋体;'>费率标准費率標準</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span
            style='font-family:宋体'>一、法幣交易費率</span></b></p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>1</span><span style='font-family:宋体'>、法幣交易區發布廣告完成交易收取廣告方交易額的 0.5% 作為手續費</span></p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>2</span><span style='font-family:宋体'>、廣告方發布買入廣告，交易手續費將從廣告方實際買入數字資產的總額中扣除，扣除的手續費以最終獲得的數字資產為標準；比如：廣告方發布買入100USDT廣告，該單全部成交後，最終廣告方獲得99.5USDT</span></p>
                                                                      
           <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>3</span><span style='font-family:宋体'>、廣告方發布賣出廣告，交易手續費將從廣告方實際賣出的數字資產中扣除，比如廣告發布賣出100USDT廣告，實際買方只能買入99.5USDT。</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span lang=EN-US
                                                                         style='font-family:宋体'>&nbsp;</span></b></p>

          <p class=MsoNormal align=left style='text-align:left;'><b><span lang=EN-US style='font-family:宋体'>二、</span></b><b><span
            style='font-family:宋体'>幣幣交易費率</span></b></p>

          <!--<p class=MsoNormal align=left style='text-align:left;'><span-->
            <!--lang=EN-US style='font-family:宋体;'>1</span><span-->
            <!--style='font-family:宋体;'>、币币交易（不含<span lang=EN-US>GCX)</span>手续费全免；</span></p>-->

          <!--<p class=MsoNormal align=left style='text-align:left;'><span-->
            <!--lang=EN-US style='font-family:宋体;'>2</span><span-->
            <!--style='font-family:宋体;'>、<span lang=EN-US>GCX</span>交易手续费<span-->
            <!--lang=EN-US>1%</span>；</span></p>-->

          <table class=MsoNormalTable border=1 cellspacing=0 cellpadding=0 align=left
                 width=0 style='border-collapse:collapse;border:none;'>
            <tr style='height:18.45pt'>
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;padding:
  0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>&nbsp;</span>
              </td>
              <td width=200 style='width:149.9pt;border:dotted windowtext 1.0pt;border-left:
  none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span style='font-family:宋体;'>掛單</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>吃單</span>
              </td>
            </tr>
            <tr style="height: 18.45pt" v-for="(item,index) in symbol">
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;border-top:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span lang=EN-US style='font-family:宋体;'>{{item.symbol}}</span>
              </td>
              <td width=200 style='width:149.9pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span lang=EN-US style='font-family:宋体;'>{{parseFloat(item.fee*100) + "%"}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span lang=EN-US style='font-family:宋体;'>{{parseFloat(item.fee*100) + "%"}}</span>
              </td>
            </tr>
          </table>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>1</span><span style='font-family:宋体'>、掛單是平臺幣幣交易用戶所下的限價單並未與當前掛單成交，並被放在買賣盤中等待成交的擺單，它增加了買賣盤的流動性。</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>2</span><span style='font-family:宋体'>當平臺幣幣交易用戶A擺單主動與平臺交易幣幣用戶 B 擺單匹配成交，用戶 B 將支付掛單交易手續費（請註意當用戶 A 限價單與用戶 B 限價單成交，而用戶A下單時間又早於用戶 B 時，用戶 B 將支付吃單費）。</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>3</span><span style='font-family:宋体'>、吃單是平臺幣幣交易用戶所下的限價單或市價單與當前的掛單直接成交</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>4</span><span style='font-family:宋体'>、當平臺幣幣交易用戶所下的擺單主動與平臺其他幣幣交易用戶的擺單成交</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>5</span><span style='font-family:宋体'>、交易手續費將從平臺幣幣交易用戶的成交總額中扣除，扣除的手續費以最終獲得的數字資產為標準；比如該用戶以單價 100 USDT 買入 1 BTC，會扣除 0.002 BTC 作為手續費，實際獲得 0.998 BTC；反之以 1 BTC買入 100 USDT,則會扣除 0.2 USDT作為手續費，實際獲得99.8 USDT。</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span
            style='font-family:宋体'>三、充幣、提幣費率</span></b><b><span
            style='font-family:宋体'>费率</span></b></p>

          <table class=MsoNormalTable border=1 cellspacing=0 cellpadding=0 align=left
                 width=0 style=';border-collapse:collapse;border:none;'>
            <tr style='height:18.45pt'>
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;padding:
  0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>&nbsp;</span>
              </td>
              <td width=200 style='width:149.9pt;border:dotted windowtext 1.0pt;border-left:
  none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>是否允許提幣</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>提币手續費</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>最小提幣數量</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>是否允許充幣</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>充幣手續費</span>
              </td>
            </tr>
            <tr style="height: 18.45pt" v-for="(item,index) in fee">
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;border-top:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.name}}</span>
              </td>
              <td width=200 style='width:149.9pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.enableWithdraw}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.withdrawFee}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.minWithdrawAmount}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.enableRecharge}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.rechargeFee}}</span>
              </td>
            </tr>
          </table>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <!-- <p class=MsoNormal align=left style='text-align:left;'><b><span
            style='font-family:宋体;'>四、提币费率</span></b></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            style='font-family:宋体'>提币平台不收取任何费用，但您需要支付矿工费。</span></p> -->

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

        </div>

      </div>
    </div>


    
    <!-- 英文 -->
     <div class="content" v-if="lang=='English'?true:false">
      <div class="agreen-cont ">

        <div class=WordSection1 style='layout-grid:15.6pt'>

          <p class=MsoNormal><span lang=EN-US style='font-family:宋体;'>Standard rates</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span
            style='font-family:宋体'>1. Rate of fiat transaction. </span></b></p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>1</span><span style='font-family:宋体'>. The fiat trading zone shall charge 0.5% of the total amount of the advertising transaction as the transaction fee.</span></p>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>2</span><span style='font-family:宋体'>. Advertisers shall issue buy-in advertisements. Transaction fee shall be deducted from the actual dealing amount of the digital assets; for example, the advertiser shall issue a buy-in 100USDT advertisement. After the transaction is completed, the advertiser gets 99.5USDT at last. </span></p>
                                                                      
           <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>3</span><span style='font-family:宋体'>. Advertisers shall issue sell-out advertisements. Transaction fee shall be deducted from the actual dealing amount of the digital assets; for example, the advertiser shall issue a sell-out 100USDT advertisement. After the transaction is completed, the buyer purchased 99.5USDT at last. </span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span lang=EN-US
                                                                         style='font-family:宋体'>&nbsp;</span></b></p>

          <p class=MsoNormal align=left style='text-align:left;'><b><span lang=EN-US style='font-family:宋体'>2. Rate of cryptocurrency. </span></b></p>

          <!--<p class=MsoNormal align=left style='text-align:left;'><span-->
            <!--lang=EN-US style='font-family:宋体;'>1</span><span-->
            <!--style='font-family:宋体;'>、币币交易（不含<span lang=EN-US>GCX)</span>手续费全免；</span></p>-->

          <!--<p class=MsoNormal align=left style='text-align:left;'><span-->
            <!--lang=EN-US style='font-family:宋体;'>2</span><span-->
            <!--style='font-family:宋体;'>、<span lang=EN-US>GCX</span>交易手续费<span-->
            <!--lang=EN-US>1%</span>；</span></p>-->

          <table class=MsoNormalTable border=1 cellspacing=0 cellpadding=0 align=left
                 width=0 style='border-collapse:collapse;border:none;'>
            <tr style='height:18.45pt'>
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;padding:
  0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>&nbsp;</span>
              </td>
              <td width=200 style='width:149.9pt;border:dotted windowtext 1.0pt;border-left:
  none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span style='font-family:宋体;'>Are cancelled</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>Taker </span>
              </td>
            </tr>
            <tr style="height: 18.45pt" v-for="(item,index) in symbol">
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;border-top:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span lang=EN-US style='font-family:宋体;'>{{item.symbol}}</span>
              </td>
              <td width=200 style='width:149.9pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span lang=EN-US style='font-family:宋体;'>{{parseFloat(item.fee*100) + "%"}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                  <span lang=EN-US style='font-family:宋体;'>{{parseFloat(item.fee*100) + "%"}}</span>
              </td>
            </tr>
          </table>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>


          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>1</span><span style='font-family:宋体'>.Maker fees are paid when you add liquidity to our order book, by placing a limit order under the last trade price for buy and above the last trade price for sell.</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>2</span><span style='font-family:宋体'>.Taker fees are paid when user A remove liquidity from our DBEX’s order book, by placing any order that is executed against an order of the orderbook. (Please note when user A limit order is executed against user B’s limit order and user A’s order placed earlier than user B’s order, user B will pay taker fees.)</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>3</span><span style='font-family:宋体'>.Taker means that the limit order or market order you place is executed with the current maker in DBEX.</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>4</span><span style='font-family:宋体'>.When the order DBEX user placed is filled by orders from other trading zones, the user needs to pay the taker fees.</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>5</span><span style='font-family:宋体'>.Trading fees will be deducted from you executed total. If user A exchange 100 USDT to 1 BTC, user A need to pay 0.002 BTC as transactions fees and gets 0.998 BTC in the end. Vice versa, if user A exchange 1 BTC to 100 USDT, user A needs to pay 0.2 USDT as transaction fee and gets 99.8 USDT at last. </span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left'><b><span
            style='font-family:宋体'>3. Trading Fees</span></b><b><span
            style='font-family:宋体'>Fee</span></b></p>

          <table class=MsoNormalTable border=1 cellspacing=0 cellpadding=0 align=left
                 width=0 style=';border-collapse:collapse;border:none;'>
            <tr style='height:18.45pt'>
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;padding:
  0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>&nbsp;</span>
              </td>
              <td width=200 style='width:149.9pt;border:dotted windowtext 1.0pt;border-left:
  none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>Withdrawal</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>Transaction Fee</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>Minimum Withdrawal</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>Deposit</span>
              </td>
              <td width=239 style='width:179.35pt;border:dotted windowtext 1.0pt;
  border-left:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span style='font-family:宋体;'>Deposit Transaction Fee</span>
              </td>
            </tr>
            <tr style="height: 18.45pt" v-for="(item,index) in fee">
              <td width=131 style='width:98.0pt;border:dotted windowtext 1.0pt;border-top:none;padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.name}}</span>
              </td>
              <td width=200 style='width:149.9pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.enableWithdraw}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.withdrawFee}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.minWithdrawAmount}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.enableRecharge}}</span>
              </td>
              <td width=239 style='width:179.35pt;border-top:none;border-left:none;
  border-bottom:dotted windowtext 1.0pt;border-right:dotted windowtext 1.0pt;
  padding:0cm 18.0pt 0cm 18.0pt;height:18.45pt'>
                <span lang=EN-US style='font-family:宋体;'>{{item.rechargeFee}}</span>
              </td>
            </tr>
          </table>

          <p class=MsoNormal align=left style='text-align:left'><span lang=EN-US
                                                                      style='font-family:宋体'>&nbsp;</span></p>

          <!-- <p class=MsoNormal align=left style='text-align:left;'><b><span
            style='font-family:宋体;'>四、提币费率</span></b></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            style='font-family:宋体'>提币平台不收取任何费用，但您需要支付矿工费。</span></p> -->

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

          <p class=MsoNormal align=left style='text-align:left;'><span
            lang=EN-US style='font-family:宋体'>&nbsp;</span></p>

        </div>

      </div>
    </div>
  </div>
</template>
<style scoped>
  .agreement {
    /* background: #fff; */
    padding-bottom: 20px;
    overflow-x:hidden;
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
    /*font-size:12px;*/
  /*}*/
  /*.content h3{*/
    /*font-size: 16px;*/
    /*padding-top: 10px;*/
  /*}*/
  .content table{
    margin: 10px 0;
    width: 100%;
    border: 1px solid #e6e6e6;
    border-spacing: 0;
    border-collapse: collapse;
  }
  .content table th,
  .content table td{
    border: 1px solid #665F57 !important;
    font-weight: normal;
    padding: 0 24px;
    line-height: 36px;
    text-align: center;
  }

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
    data(){
      return {
        symbol:[],
        fee:[]
      }
    },
    mounted:function () {
      this.getSymbol();
      this.getWithdrawFee();
    },
    methods:{
      getSymbol:function () {
        this.$http.post(this.host + '/market/symbol').then(response => {
          var result = response.body;
          this.symbol = result;
        });
      },
      getWithdrawFee:function () {
        this.$http.post(this.host + '/uc/coin/supported').then(response => {
            var result = response.body;
            this.fee = result;
            this.convertFee()
        })
      },
      convertFee:function () {
        for (var i = 0 ; i < this.fee.length ; i++) {
          switch (this.fee[i].name){
            case "Bitcoin":
              this.fee[i].name = "BTC";
              break;
            case "Bitcoincash":
              this.fee[i].name = "BCH";
              break;
            case "Ethereum":
              this.fee[i].name = "ETH";
              break;
            case "GalaxyChain":
              this.fee[i].name = "GCC";
              break;
            case "Litecoin":
              this.fee[i].name = "LTC";
              break;
          }

          switch (this.fee[i].enableWithdraw) {
            case "1":
              this.fee[i].enableWithdraw = "允许";
              break;
            default:
              this.fee[i].enableWithdraw = "不允许";
              break;
          }

          switch (this.fee[i].enableRecharge) {
            case "1":
              this.fee[i].enableRecharge = "允许";
              break;
            default:
              this.fee[i].enableRecharge = "不允许";
              break;
          }

          if (this.fee[i].withdrawFee.indexOf("E-") > -1) {
            var leftV = parseFloat(this.fee[i].withdrawFee.split("E-")[0]);
            var rightV = parseFloat(this.fee[i].withdrawFee.split("E-")[1]);
            for (var s=0;s<rightV;s++) {
              leftV = leftV / 10;
            }
            this.fee[i].withdrawFee = leftV;
          }

          this.fee[i].rechargeFee = 0;
        }
      },
      getFeeBySymbol:function (coin) {
        var fee = '0%';
        for (var i=0;i<this.symbol.length;i++){
            if(this.symbol[i].symbol == coin){
              fee = parseFloat(this.symbol[i].fee*100) + "%";
              break;
            }
        }
        return fee;
      }
    },
  computed:{
     lang() {
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
