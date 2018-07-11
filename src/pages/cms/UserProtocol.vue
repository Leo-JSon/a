<template>
  <div class="agreement">
    <img src="../../assets/images/call.png">
    <div class="agreement_tab">
      <div class="static_main">
        <router-link to="/about-rule">{{$t('cms.exchangerule')}}</router-link>
        <router-link to="/about-protocol" class="cur">{{$t('cms.useprotocol')}}</router-link>
        <router-link to="/about-fee">{{$t('cms.feenote')}}</router-link>
        <!-- <router-link to="/about-merchant">{{$t('cms.merchantprocotol')}}</router-link> -->
      </div>
    </div>
      <div class="content">
            <div class='WordSection1' style='layout-grid:15.6pt'>
        
          <p class='MsoNormal' align='left' style='text-align:left'><span lang=EN-US style='font-family:宋体'>&nbsp;</span></p>
          </div>
            <div class='WordSection1' style='layout-grid:15.6pt' v-if="lang!='English'">
              <div >https://www.bcuae.pro.com（以下稱“本網站”或“網站”）是由 Block Chain Group Holding LTD。（以下稱“公司”）運營的網站，該網站是一個專門供用戶進行數字資產交易和提供相關服務（以下稱“該服務”或“服務”）的平台。為了本協議表述之方便，公司和該網站在本協議中合稱使用“我們”或其他第一人稱稱呼。只要登陸該網站的自然人或其他主體均為本網站的用戶，本協議表述之便利，以下使用“您”或其他第二人稱。為了本協議表述之便利，我們和您在本協議中合稱為“雙方”，我們或您單稱為“一方”。
              </div>
              <em class="paragraph">重要提示</em>
              
              <ul>
                <li>我們在此特別提醒您：</li>
                <li>1.數字資產本身不由任何金融機構或公司或本網站發行;</li>
                <li>2.數字資產市場是全新的，未經確認的，而且可能不會增長;</li>
                <li>3.數字資產主要由投資者大量使用，零售和商業市場使用相對較少，數字資產交易存在極高風險，其全天不間斷交易，沒有漲跌限制，價格容易受莊家，全球政府政策的影響而大幅波動;</li>
                <li>4.因各國法律，法規和規範性文件的製定或者修改，數字資產交易隨時可能被暫停或被禁止。</li>
              </ul>
           
              <ul>
                <li>數字資產交易有極高風險，並不適合絕大部分人士。您了解和理解此投資有可能導致部分損失或全部損失，所以您應該以能承受的損失程度來決定投資的金額。您了解和理解數字資產會產生衍生風險，所以如有任何疑問，建議先尋求理財顧問的協助。此外，除了上述提及過的風險以外，還會有未能預測的風險存在。您應慎重考慮並用清晰的判斷能力去評估自己的財政狀況及上述各項風險而作出任何買賣數字資產的決定，並承擔由此產生的全部損失，我們對此不承擔任何責任。</li>
              <li>敬告您</li>	
                <li>1.您了解本網站僅作為您獲取數字資產信息，尋找交易方式，就數字資產的交易進行協商及開展交易的場所，本網站不參與您的任何交易，故您應自行謹慎判斷確定相關數字資產及/或信息的真實性，合法性和有效性，並自行承擔因此產生的責任與損失。
                </li>
                <li>2.本網站的任何意見，消息，探討，分析，價格，建議和其他資訊均為一般的市場評論，並不構成投資建議。但不限於任何利潤損失。</li>
                <li>3.本網站的內容會隨時更改並不作另行通知，我們已採取合理措施確保網站資訊的準確性，但並不能保證其準確性，亦不會承擔任何因本網站上的資訊或因未能鏈結互聯網，傳送或接收任何通知和信息時的延誤或失敗而直接或間接產生的損失。
                </li>
                <li>4.使用互聯網形式的交易系統亦存在風險，包括但不限於軟件，硬件和互聯網鏈接的失敗等。由於我們不能控制互聯網的可靠性和可用性，我們不會對失真，延誤和鏈結失敗而承擔任何責任。</li>
                <li>
                    5.https://www.bcuae.pro.com/為本網站唯一官方對外信息公佈平台;
                </li>
                <li>6. 本網站任何服務均不受信用卡支付;
                </li>
                <li>7. 禁止使用本網站從事洗錢，走私，商業賄賂等一切非法交易活動，若發現此類事件，本站將採取各種可使用之手段，包括但不限於凍結賬戶，通知相關權力機關等，我們不承擔由此產生的所有責任並保留向相關人士追究責任的權利。</li>
                
              </ul>
              <em class="paragraph">一、總則</em>
              <ul>
                <li>1.1 “用戶協議”（以下稱“本協議”或“本條款及條件”），由正文，“隱私條款”，“了解你的客戶和反洗錢政策”以及本網站已經發布或將來可能發布的各類規則，聲明，說明等構成。</li>
                <li>1.2 您在本網站提供的各項服務之前，應仔細閱讀本協議，如有不理解之處或其他必要，請諮詢專業律師。如您不同意本協議及/或隨時對其修改，請您立即停止使用本網站提供的服務或不再登陸本網站。您一旦登陸本網站，使用本網站的任何服務或任何其他類似行為即表示您已了解並完全同意本協議各項內容，包括本網站對本協議隨時所做的任何修改。
                </li>
                <li>1.3 您通過按照本網站的要求填寫相關信息，並經過其他相關程序後成功註冊可以成為本網站的會員（以下稱“會員”），在進行註冊過程中點擊“同意”按鈕即表示您以電子簽署的形式與公司達成協議;或您在使用本網站過程中點擊任何標有“同意”或類似意思的按鈕的行為或以其他本網站允許的方式實際使用本網站提供的服務時，均表示您完全了解，同意且接受本協議項下的全部條款的約束，無您手寫的書面簽字就本協議對您的法律約束力無任何影響。
                </li>
                <li>1.4 您成為本網站的會員後，您將獲得一個會員帳號及相應的密碼，該會員帳號和密碼由會員負責保管;會員應當對其以下帳戶進行的所有活動和事件負法律責任。</li>
                <li>1.5 只有成為本網站的會員才可使用本網站提供的數字資產交易平台進行交易及享受其他本網站規定的只有會員才可獲得的服務;會員外部的其他本網站及其他本網站規定的可獲得的服務。</li>
                <li>
                  <p>1.6 通過註冊和使用任何本網站提供的服務和功能，您將被視為已閱讀，理解並：</p>
                  <ul class="indent">
                    <li>1.6.1 接受本協議所有條款及條件的約束</li>
                    <li>1.6.2 您確認您已年滿16周歲或根據不同的可適用的法律規定的具有可訂立合同的法定年齡，並有充分的能力接受這些條款，並訂定交易，使用本網站進行數字資產交易。</li>
                    <li>1.6.3 您保證交易中涉及到的屬於您的數字資產均為合法取得併所有。</li>
                    <li>1.6.4 您同意您為您自己的交易或非交易行為承擔全部責任和任何收益或虧損。</li>
                    <li>1.6.5 您確認註冊時提供的信息是真實和準確的</li>
                    <li>1.6.6 您同意遵守任何有關法律的規定，就稅務目的而言，包括任何交易利潤。</li>
                    <li>1.6.7 本協議只是就您與我們之間達成的權利義務關係進行約束，而並不涉及本網站用戶之間與其他網站和您之間因數字資產交易而產生的法律關係及法律糾紛。</li>
                  </ul>
                </li>
              </ul>
              <em class="paragraph">二，協議修訂</em>
              <div>
              我們保留不時修訂本協議，並以網站公示的方式進行公告，不再單獨通知您的權利，變更後的協議會在本協議首頁標註變更時間，一經在網站公佈，立即自動生效。您應不時瀏覽及關注本協議的更新變更時間及更新內容，如您不同意相關變更，應當立即停止使用本網站服務;您繼續使用本網站服務，即表示您接受並同意經修訂的協議的約束。
              </div>
              <em class="paragraph">三，註冊</em>
              <ul>
                <li>3.1 注册资格</li>
                <li>
                3.1 您確認並承諾：在您完成註冊程序或以其他本網站允許的方式實際使用本網站提供的服務時，您應當是具備可適用的法律規定的可簽署本協議及使用本網站服務應具有的能力的自然人，法人或其他組織。您一旦點擊同意註冊按鈕，即表示您自身或您的有權代理人已經同意該協議內容並由其代理註冊及使用本網站服務。若您不具備前述主體資格，則您及您的有權代理人應承擔因此而導致的一切後果，且公司保留註銷或永久凍結您賬戶，並向您及您的有權代理人追究責任的權利。
                </li>
                <li>3.2 注册目的</li>
                <li>3.2您確認並承諾：您進行本網站註冊並非出於違反法律法規或破壞本網站數字資產交易秩序的目的。</li>
                <li>
                  <p>3.3註冊流程</p>
                  <ul class="indent">
                    <li> 3.3.1您同意根據本網站用戶註冊頁面的要求提供有效電子郵箱，手機號碼等信息，您可以使用您提供或確認的郵箱，手機號碼或者本網站允許的其它方式作為登陸手段進入本網站。如有必要，按照不同法域相關法律法規的規定，您必須提供您的真實姓名，身份證件等法律法規及隱私條款及反洗錢條款規定的相關信息並不斷更新註冊資料，符合及時，詳盡，準確的要求。所有原始鍵入的資料將引用為註冊資料。您應對該等信息的真實性，完整性和準確性負責，並承擔因此產生的任何直接或間接損失及不利後果。
                    </li>
                    <li>3.3.2如您所在的主權國家或地區的法律法規，規則，命令等規範對手機號碼有實名要求，您同意提供註冊的手機號碼是經過實名登記的，如您不按照規定提供，因此給您帶來的任何直接或間接損失及不利後果均應由您承擔。
                    </li>
                    <li>3.3.3 您合法，完整並有效提供註冊所需信息並經驗證，有權獲得本網站賬號和密碼，您獲得本網站賬號及密碼時視為註冊成功，可在本網站進行會員登陸。</li>
                    <li>3.3.4您同意接收本網站發送的與本網站管理，運營相關的電子郵件和/或短消息。</li>
                  
                  </ul>
                </li>
              </ul>
             <ul>
               <li>
                 <pre style='white-space: pre-wrap;'>
<em class="paragraph">四，服務</em>
  本網站只為您通過本網站進行數字資產交易活動（包括但不限於數字資產交易等服務）提供網絡交易平台服務，本網站並不作為買家或賣家參與買賣數字資產行為本身;本網站不提供任何國家法定貨幣充入和提取的相關服務。
  4.1服務內容<br/>
  4.1.1您有權在本網站瀏覽數字資產的各項產品的實時行情及交易信息，有權通過本網站提交數字資產交易指令並完成數字資產交易。<br/>

  4.1.2您有權在本網站查看其本網站會員賬號的信息，有權應用本網站提供的功能進行操作。<br/>

  4.1.3您有權按照本網站發布的活動規則參與本網站組織的網站活動。<br/>

  4.1.4本網站承諾為您提供的其他服務。<br/>

  4.2。服務規則<br/>

  您承諾遵守下列本網站服務規則：
  4.2.1您應當遵守法律法規，規章和政策要求的規定，保證賬戶中所有數字資產來源的合法性，不得在本網站或利用本網站服務從事非法或其他損害本網站或第三方權益的活動，如發送或接收任何違法，違規，侵犯他人權益的信息，發送或接收傳銷材料或存在其他危害的信息或言論，未經本網站授權使用或偽造本網站電子郵件題頭信息等。<br/>

  4.2.2您應當遵守法律法規並妥善使用和保護本網站賬號及登錄密碼，資金密碼及其註冊時綁定的手機號碼，以及手機接收的手機驗證碼的安全。您對本使用其本網站賬號和登陸密碼，資金密碼，手機驗證碼進行的任何操作和後果承擔全部責任。當您發現本網站賬號，登陸密碼，或資金密碼，驗證碼被未經其授權的第三方使用，或存在其他賬號安全問題時，應立即有效通知本網站，要求本網站暫停本網站賬號的服務。本網站有權在合理時間內對您的該等請求採取行動，但本網站對在採取行動前已經產生的後果（包括但不限於您的任何損失）不承擔任何責任。您在未經本網站同意的情況下不得將本網站賬號以贈與，借用，租用，轉讓或其他方式處分給他人。<br/>

  4.2.3您同意您對本網站的賬號，密碼下發生的所有活動（包括但不限於信息披露，發布信息，網上點擊同意或提交各類規則協議，網上續簽協議或購買服務等）承擔責任。<br/>

  4.2.4您在本網站進行數字資產交易時不得惡意干擾數字資產交易的正常進行，破壞交易秩序;不得以任何技術手段或其他方式乾擾本網站的正常運行或乾擾其他用戶對本網站服務的使用;不得以虛構事實等方式惡意詆毀本網站的商譽。<br/>

  4.2.5如您因網上交易與其他用戶產生糾紛的，不得通過司法或行政以外的途徑要求本網站提供相關資料。<br/>

  4.2.6您在使用本網站提供的服務過程中，所產生的應納稅賦，以及一切硬件，軟件，服務及其它方面的費用，均由您獨自承擔。<br/>

  4.2.7您應當遵守本網站不時發布和更新的本協議以及其他服務條款和操作規則，有權隨時終止使用本網站提供的服務。<br/>

  4.3。產品規則<br/>

  4.3.1幣幣交易產品規則
  您承諾在其進入本網站交易，通過本網站與其他用戶進行幣幣交易的過程中良好遵守如下交易規則。

  4.3.1.1瀏覽交易信息
  在本網站瀏覽幣種交易信息時，應當仔細閱讀交易信息中包含的全部內容，包括但不限於價格，委託量，手續費，買入或賣出方向，您完全接受交易信息中包含的全部內容後方可點擊按鈕進行交易。

  4.3.1.2提交委託
  在瀏覽完交易信息確認無誤之後您可以提交交易委託。您提交交易委託後，即您授權本網站代理您進行相應的交易撮合，本網站在有滿足您委託價格的交易時將會自動完成撮合交易而無需提前通知您。

  4.3.1.3查看交易明細
  您可以通過管理中心的交易明細中查看相應的成交記錄，確認自己的詳情交易記錄。

  4.3.1.4撤銷/修改委託，在委託未達成交易之前，您有權隨時撤銷或修改委託。
                    </pre>
                </li>
                <li>
                    <pre style="white-space: pre-wrap;">
<em class="paragraph">五，本網站的權利和義務</em>
  5.1如您不具備本協議約定的註冊資料，則本網站有權拒絕您進行註冊，對已註冊的本網站有權註銷您的會員賬號，本網站保留向您或您的有權代理人追究責任的權利。同時，本網站保留其他任何情況下決定是否接受您註冊的權利。

  5.2本網站發現賬戶使用者並非賬戶初始註冊人時，有權中止或終止該賬戶的使用。

  5.3本網站通過技術檢測，人工抽檢等檢測方式合理懷疑您提供的信息錯誤，不實，失效或不完整時，有權通知您更正，更新信息或中止，終止為其提供本網站服務。

  5.4本網站有權在發現本網站上顯示的任何信息存在明顯錯誤時，對信息予以更正。

  5.5本網站保留隨時修改，中止或終止本網站服務的權利，本網站行為修改或中止服務的權利不需事先告知您;本網站終止本網站一項或多項服務的，終止本本網站在網站上發布終止公告之日生效。

  5.6本網站應當採取必要的技術手段和管理措施保障本網站的正常運行，並提供必要的可靠交易環境和交易服務，維護數字資產交易秩序。

  5.7如您連續一年未使用本網站會員賬號和密碼登陸本網站，則本網站有權註銷您的本網站賬號。賬號註銷後，本網站有權將相應的會員名開放給其他您註冊使用。

  5.8本網站通過加強技術投入，提升安全防範等措施保證您的數字資產的安全，有義務在您賬戶出現可以預見的安全風險時提前通知您。

  5.9本網站有權隨時刪除本網站內各類不符合法律法規或本網站規定等的內容信息，本網站行使該等權利不需提前通知您。

  5.10本網站有權根據您所屬的主權國家或地區的法律法規，規則，命令等規範的要求，向您要求提供更多的信息或資料等，並採取合理的措施，以符合當地的規範之要求，您有義務配合;本網站有權根據您所屬主權國家或地區的法律法規，規則，命令等規範的要求，暫停或永久停止對您的開放本網站及其部分或全部服務。

                    </pre>
                </li>
                  <li>
                  <em class="paragraph">六，賠償</em>
                      <pre style="white-space: pre-wrap;">
6.1在任何情況下，我們對您的直接損害的賠償責任均不會超過您從本使用本網站服務產生的為期三個月的總費用。

   6.2如您發生違反本協議或其他法律法規等情況，您須向我們至少賠償200萬美元及承擔由此產生的全部費用（包括律師費等），如不夠彌補實際損失，您須補全。

                      </pre>
                  </li>
                    <li>
    <em class="paragraph">七，尋求禁令救濟的權利</em>
        <pre style="white-space: pre-wrap;">
我們和您均承認普通法對違約或可能違約情況的救濟措施是可能是不足以彌補我們遭受的全部損失的，故非違約方有權在違約或可能違約情況下尋求禁令救濟以及普通法或衡平法允許的其他所有的補救措施。
        </pre>
    </li>
      <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">八，責任限制與免責</em>
  8.1您了解並同意，在任何情況下，我們不就以下各事項承擔責任：

  8.1.1收入的損失;

  8.1.2交易利潤或合同損失;

  8.1.3業務中斷

  8.1.4預期可節省的貨幣的損失;

  8.1.5信息的損失;

  8.1.6機會，商譽或聲譽的損失;

  8.1.7數據的損壞或損失;

  8.1.8購買替代產品或服務的成本;

  8.1.9任何由於侵權（包括過失），違約或其他任何原因產生的間接的，特殊的或附帶性的損失或損害，不論這種損失或損害是否可以為我們合理預見;不論我們是否事先被告知存在此種損失或損害的可能性。

  8.1.1條至8.1.9條均是彼此獨立的。

  8.2您了解並同意，我們不對因下述任一情況而導致您的任何損害賠償承擔責任：

  8.2.1我們有合理的理由認為您的具體交易事項可能存在重大違法或違約情形。

  8.2.2我們有合理的理由認為您在本網站的行為涉嫌違法或不當。

  8.2.3通過本網站服務購買或獲取任何數據，信息或進行交易等行為或替代行為產生的費用和損失。

  8.2.4您對本網站服務的誤解。

  8.2.5任何非因我們的原因而引起的與本網站提供的服務有關的其它損失。

  8.3我們對由於信息網絡設備維護，信息網絡連接故障，電腦，通訊或其他系統的故障，電力故障，天氣原因，意外事故，罷工，勞動爭議，暴亂，起義，騷亂，生產力或生產資料不足，火災，洪水，風暴，爆炸，戰爭，銀行或其他合作方原因，數字資產市場崩潰，政府行為，司法或行政機關的命令，其他不在我們可控範圍內或我們無能力控制的行為或第三方的原因而造成的不能服務或延遲服務，以及造成的您的損失，我們不承擔任何責任。

  8.4我們不能保證本網站包含的全部信息，程序，文本等完全安全，不受任何病毒，木馬等惡意程序的干擾和破壞，故您的登陸，使用本網站任何服務或下載及使用該下載的任何程序，信息，數據等均是您個人的決定並自行承擔風險及可能產生的損失。

  8.5我們對本網站中鏈接的任何第三方網站的任何信息，產品及業務及其他任何形式的不屬於我們的主體的內容等不做任何保證和承諾，您如果使用第三方網站提供的任何服務，信息及產品等均為您個人決定且承擔由此產生的一切責任。

  8.6我們對於您使用本網站服務不做任何明示或暗示的保證，包括但不限於本網站提供的服務的適用性，沒有錯誤或疏漏，持續性，準確性，可靠性，適用於某一特定用途。同時，我們也不對本網站提供的服務所涉及的技術及信息的有效性，準確性，正確性，可靠性，質量，穩定，完整和及時性作出任何承諾和保證。是否登陸或使用本網站提供的服務是您個人的決定且自行承擔風險及可能產生的損失。我們對於數字資產的市場，價值及價格等不做任何明示或暗示的保證，您理解並了解數字資產市場是不穩定的，價格和價值隨時會大幅波動或崩盤，交易數字資產是您個人的自由選擇及決定且自行承擔風險及可能產生的損失。

  8.7本協議中規定的我們的保證和承諾是由我們就本協議和本網站提供的服務的唯一保證和陳述，並取代任何其他途徑和方式產生的保證和承諾，無論是書面的或口頭的，明示的或暗示的。所有這些保證和陳述僅僅代表我們自身的承諾和保證，並不保證任何第三方遵守本協議中的保證和承諾。

  8.8我們並不放棄本協議中未提及的在法律適用的最大範圍內我們享有的限制，免除或抵銷我們損害賠償責任的任何權利。

  8.9您註冊後即表示認可我們按照本協議中規定的規則進行的任何操作，產生任何風險均由您承擔。

        </pre>
    </li>
      <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">九，協議的終止</em>
  9.1本網站有權依據本協議約定註銷您的本網站賬號，本協議於賬號註銷之日終止。

  9.2本網站有權依據本協議約定終止全部本網站服務，本協議於本網站全部服務終止之日終止。

  9.3本協議終止後，您無權要求本網站繼續向其提供任何服務或履行任何其他義務，包括但不限於要求本網站為您保留或向您披露其原本網站賬號中的任何信息，向您或第三方轉發任何其未曾閱讀或發送過的信息等。

  9.4本協議的終止不影響守約方向違約方要求其他責任的承擔。
        </pre>
    </li>
      <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">十，知識產權</em>
  10.1本網站所包含的全部智力成果包括但不限於網站標誌，數據庫，網站設計，文字和圖表，軟件，照片，錄像，音樂，聲音及其前述組合，軟件編譯，相關源代碼和軟件小應用程序和腳本）的知識產權權利均歸於本網站所有。您不得為商業目的複制，更改，拷貝，發送或使用前述任何材料或內容。

  10.2本網站名稱中包含的所有權利（包括但不限於商譽和商標，標誌）均歸公司所有。

  10.3您接受本協議即視為您主動將其在本網站發表任何形式的信息的權利，包括但不限於：複製權，發行權，出租權，展覽權，表演權，放映權，廣播權，信息網絡傳播權，攝製權，改編權，翻譯權，彙編權以及應當由作者權享有的其他可轉讓權利無償獨家轉讓給本網站所有，本網站有權利就任何主體侵權單獨提起訴訟並獲得全部賠償。本協議效力及於本在本網站發布的任何受版權法保護的作品內容，無論該內容形成於本協議簽訂前還是本協議簽訂後。

  10.4您在本網站服務過程中不得非法使用或處理本網站或他人的知識產權權利。您不會將本發佈於本網站的信息以任何形式發布或授權其它網站（及媒體）使用。

  10.5您登陸本網站或使用本網站提供的任何服務均不視為我們向您轉讓任何知識產權。

        </pre>
    </li>
  <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">十一，信息保護</em>
  11.1適用範圍

  11.1.1在您註冊網站賬號或者使用賬戶時，您根據本網站要求提供的個人註冊信息，包括但不限於電話號碼，郵箱信息，身份證件信息。

  11.1.2在您使用本網站服務時，或訪問本網站時，本網站自動接收並記錄您的瀏覽器上的服務器數值，包括但不限於IP地址等數據及您要求取用的網頁記錄。

  11.1.3本網站收集到的您在本網站進行交易的有關數據，包括但不限於交易記錄。

  11.1.4本網站通過合法途徑取得的其他您個人信息。

  11.2信息使用

  11.2.1不需要您額外的同意，您在本網站註冊成功即視為您同意本網站收集並使用本網站的各類信息，如11.1條所列，您了解並同意，本網站可以將收集的您信息用作包括但不限於下列用途：

  11.2.1.1向您提供本網站服務;

  11.2.1.2根據主權國家或地區相關主管部門的要求向相關部門進行報告;

  11.2.1.3在您使用本網站服務時，本網站將您的信息用於身份驗證，客戶服務，安全防範，詐騙監測，存檔和備份用途，確保本網站向您提供的產品和服務的安全性;

  11.2.1.4幫助本網站設計新產品及服務，改善本網站現有服務;

  11.2.1.5為了使您解本網站服務的具體情況，您同意本網站向其發送營銷活動通知，商業性電子信息以及提供與您相關的廣告以替代普遍投放的廣告;

  11.2.1.6本網站為完成合併，分立，收購或資產轉讓而將您的信息轉移或披露給任何非關聯的第三方;

  11.2.1.7軟件認證或管理軟件升級;

  11.2.1.8邀請您參與有關本網站服務的調查;

  11.2.1.9用於和政府機關，公共事務機構，協會等合作的數據分析;

  11.2.1.10用作其他一切合法目的以及經您授權的其他用途。

  11.2.2本網站不會向其他任何人出售或出借您的個人信息，除非事先得到您的許可。本網站也不允許任何第三方以任何手段收集，編輯，出售或者無償傳播您的個人信息。

  11.3本網站對所獲得的客戶身份資料和交易信息等進行保密，不得向任何單位和個人提供客戶身份資料和交易信息，應相關主權國家或地區法律法規，政令，命令等規定要求本網站提供的除外。

        </pre>
    </li>
      <li>
    <em class="paragraph">十二，計算所有的交易計算結果都經過我們的核實，所有的計算方法都已經在網站上公示，但是我們不能保證證書網站的使用不會受到干擾或沒有誤差。</em>
    <em class="paragraph">十三，出口控制您理解並承認，根據阿拉伯聯合酋長國相關法律，您不得將本網站上的任何材料（包括軟件）出口，再出口，進口或轉移，故您保證不會主動實施或協助或參與任何上述違反法規的出口或有關轉移或其他違反適用的法律和法規的行為;如發現此類情形，會向我們積極報告並協助我們處理。</em>
    <em class="paragraph">十四，轉讓本協議中約定的權利及義務同樣約束從該權利義務中獲取到利益的各方的受讓人，繼承人，遺囑執行人和管理員。您不得在我們不同意的前提下轉讓給任何第三人，但我們可隨時將我們在本協議中的權利和義務轉讓給任何第三人，並給予您提前30天的通知。</em>
    <em class="paragraph">十五，可分割性如本協議中的任何款被任何有管轄權的法院認定為不可執行的，無效或非法的，並不影響本協議的其餘條款的效力。</em>
    <em class="paragraph">十六，非代理關係本協議中的任何規定均不可被認為創造了，暗示了或以其他方式將我們視為您的代理人，受託人或其他代表人，本協議有其他規定的除外</em>
      <em class="paragraph">十七，棄權我們或您任何一方對追究本協議約定的違約責任或其他責任的棄權並不能認定或解釋為對其他違約責任的棄權;未行使任何權利或救濟不得以任何方式被解釋為對等的利益或救濟的放棄。不適用於擴大或限制該協議條款的內容或範圍。</em>
        <em class="paragraph">十八，標題</em>
         <pre style="white-space: pre-wrap;">
所有標題僅供協議表述方便，並不用於擴大或限制該協議條款的內容或範圍。
        </pre>
          <em class="paragraph">十九，適用法律本協議全部內容均為根據阿拉伯聯合酋長國法律訂立的合同，其成立，解釋，內容及執行均適用阿拉伯聯合酋長國相關法律規定;任何因或與本協議約定的服務有關而產生的索賠或訴訟，都應依阿拉伯聯合酋長國的法律進行管轄並加以解釋和執行。為避免疑義，這一條款明確適用於任何針對我們的侵權索賠。任何針對我們或者是和我們有關的索賠或訴訟的管轄法院或訴訟地均在阿拉伯聯合酋長國。您無條件地獲得在阿拉伯聯合酋長國法院進行訴訟和上訴的排他性的管轄權。您也無條件地同意與本協議款有關的爭議或問題或產生的任何索賠請求和訴訟的發生地或法院均排他性得在阿拉伯聯合酋長國。不方便法院的原則不適用於根據本服務條款的選擇的法院。</em>
    </li>
     <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">二十，協議的生效和解釋</em>
  20.1本協議於您點擊本站註冊頁面的同意註冊並完成註冊程序，獲得本網站賬號和密碼時生效，本網站和您均具有約束力。

  20.2本協議的最終解釋權歸本網站所有。
        </pre>
    </li>
     <li>
    <em class="paragraph">了解你的客戶和反洗錢政策</em>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">一，導言</em>
  1.1我們保證審慎遵守“了解你的客戶”和反洗錢相關的法律法規且不得故意違反該“了解你的客戶和反洗錢政策”。在我們合理控制的範圍內我們將採取必要的措施和技術為您提供安全的服務，盡可能使您免於遭受犯罪嫌疑人的洗錢行為帶來的損失。

  1.2我們的了解你的客戶和反洗錢政策是一個綜合性的國際政策體系，包括您隸屬的不同法律轄區的了解你的客戶和反洗錢政策。我們健全合規的框架確保我們在本地和全球層面均符合監管要求和監管水平，並確保本網站持續性運行。

        </pre>
    </li>
     <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">二，了解你的客戶和反洗錢政策如下：</em>
  2.1頒布了解你的客戶和反洗錢政策並時時更新以滿足相應的法律法規規定的標準;

  2.2頒布和更新運行本網站的一些指導原則和規則，且我們的員工將按照該原則和規則的指導提供服務;

  2.3設計並完成內部監測和控制交易的程序，如以嚴格的手段驗證身份，安排組建專業團隊專門負責反洗錢工作;

  2.4採用風險預防的方法對客戶進行盡職調查和持續的監督;

  2.5審查和定期檢查已發生的交易;

  2.6向主管當局報告可疑交易;

  2.7身份證明文件，地址證明文件和交易記錄的證明文件將會維持至少六年，如被提交給監管部門，恕不另行通知您。

  2.8整個交易過程中，信用卡被禁止使用;
        </pre>
    </li>
     <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">三，身份信息與核實確認</em>
  3.1身份信息
  3.1.1根據不同的司法管轄區的不同的規定及不同的實體類型，我們收集的您的信息內容可能不一致，原則上將向註冊的個人收集以下信息：
  個人基本信息：您的姓名，住址（及永久地址，如果不同），出生日期及國籍等可獲得的其他情況身份驗證應該是根據官方或其他類似權威機構發放的文件，比如護照，身份證或其他不同的轄區要求的和引發的身份證明文件。您提供的地址將使用適當的方法進行驗證，比如檢查乘用交通工具的票據或利率票據或檢查選民登記冊等。
  有效的照片：在您註冊之前，您須提供您將您的身份證件放在胸前的照片;
  聯繫方式：電話/手機號碼和/或有效的電子郵件地址。

  3.1.2如果您是一個公司或其他合法實體，我們將收集以下信息以確定您或信託帳戶的最終受益人。
  公司註冊，登記證;公司的章程與備忘錄副本;公司的股權機構和所有權說明的詳細證明材料，證明決定本網站賬戶的開立以及執行的授權委託人的董事會決議;按照要求需要提供的公司董事，大股東及本網站賬戶有權簽字人的身份證明文件。該公司的主要營業地址，如果與公司的郵寄地址不同，提供郵寄地址如果公司在本地的地址與它的主要營業地址不一致的，則被視為風險較高的客戶，需要提交額外附加文件。
  根據不同的司法管轄區的不同規定及不同的實體類型，我們要求的其他認證和權威部門發布的文件以及我們認為必要的文件。

  3.1.3我們只接受英語版或英文版本的身體信息，如不是，請您將您的身體信息翻譯成英文的版本並加以公證。

  3.2確認核實

  3.2.1我們要求您提供身份證明文件的全部頁面內容。

  3.2.2我們要求您提供您將您的身份證明文件放在您胸前的照片。

  3.2.3證明文件的副本一般應核和原始憑證進行核對。然而，如果某個可信賴的合適的認證人可證明該副本文件是原始文件準確而全面的複製的，該副本可接受。這樣的認證人包括大使，司法委員，地方治安官等。

  3.2.4對識別最終受益人和賬戶控制權的要求是確定哪些個人最終所有或控制直接客戶，和/或確定正在進行的交易是由他人代為執行。如果是企業，則大股東的身份例如那些持有10％或以上的投票權益）應被驗證一般，持股25％會被認定為正常風險內，其股東身份須驗證;持股10％或擁有更多的投票權或股票時被認定為高風險的情況，股東身份須加以驗證。
        </pre>
    </li>
      <li>
        <pre style="white-space: pre-wrap;">
    <em class="paragraph">四，監控交易</em>
  4.1我們根據安全性和實際交易情況時間設置和調整日常交易和提幣最高限額;
  4.2如果交易頻繁集中發生在某個註冊用戶或存在超乎合理的情況，我們的專業團隊將評估並決定他們是否可疑;
  4.3我們憑藉自身的判斷認定為可疑交易的情況，我們可能會採取暫停該交易，拒絕該交易等限制性措施，甚至如果可能將盡快逆轉該交易，同時向主管部門報告，但不會通知您;
  4.4我們保留拒絕來自於不符合國際反洗錢標準轄區的人或可被視為政治公眾人物的人的註冊申請，我們保留隨時暫停或終止根據我們自身判斷為可疑交易的交易，但我們這樣做並不違反對您的任何義務和責任。
        </pre>
    </li>
  <li>
    <em class="paragraph">風險提示</em>
    <em class="paragraph"> 一，系統性風險</em>
        <pre style="white-space: pre-wrap;">
指由於全局性的共同因素引起的收益的可能變動，這種因素以同樣的方式對所有證券/非證券的收益產生影響。例如市場風險中，若數字資產市場整體價值被高估，那麼投資風險將加大，參與者可能會對項目的期望過高，但這些高期望可能無法實現。同時，系統性風險還包括一系列不可抗力因素，包括且不僅限於地震，火災等自然災害，計算機網絡在全球範圍內的大規模故障和政治動盪等。
        </pre>
    </li>
      <li>
    <em class="paragraph">二，團隊風險</em>
        <pre style="white-space: pre-wrap;">
登錄EXCUAE交易所的項目方均承諾其團隊由區塊領域的資深從業者，具有豐富經驗的技術開發人員等組成。在項目的發展中，不排除有團隊核心人員離開，團隊內部發生衝突而導致項目整體發展受到負面影響的可能性。
        </pre>
    </li>
      <li>
    <em class="paragraph">四，項目統籌，營銷風險</em>
        <pre style="white-space: pre-wrap;">
登錄DBEX交易所的項目方均承諾，其項目的生態社區將不遺餘力實現白皮書中所提出的發展目標及延展項目的可成長空間。而鑑於行業整體發展趨勢存在不可預見因素，現有的商業模型與統籌思路存在與市場需求不能良好吻合從而導致項目運行難以出現可觀的成果。同時，由於本白皮書可能隨著項目細節的更新而進行調整，如果私募參與者未能及時獲取項目更新的相關細節，或是公眾對項目的最新進展不了解，參與者或公眾因信息不對稱造成對項目認知不足，從而影響到項目的後續發展。
        </pre>
    </li>
      <li>
    <em class="paragraph">五，黑客攻擊與犯罪風險</em>
        <pre style="white-space: pre-wrap;">
在安全性方面，加密數字代幣具有匿名性，難以追溯等特點，易被犯罪分子所利用，或受到黑客攻擊，或可能涉及到非法資產轉移等犯罪行為。
        </pre>
    </li>
    <li>
    <em class="paragraph">六，目前尚未可知的其他風險</em>
        <pre style="white-space: pre-wrap;">
隨著區塊鏈技術與行業整體態勢的不斷發展，EXCUAE可能會面臨一些尚未遇到的風險。請參與者在做出參與決策之前，充分了解項目內容，知曉項目整體框架與思路，合理調整自己的願景。
        </pre>
    </li>
    <li>
    <em class="paragraph">免責聲明</em>
        <pre style="white-space: pre-wrap;">
本文檔僅作為傳達信息之用，文檔內容僅供參考，不構成在EXCUAE的可投資買賣建議，教睃或邀約。參與EXCUAE線上交易則代表參與者已達到年齡標準，具備完整的民事行為能力，完全認可EXCUAE用戶協議.DBEX交易的所有虛擬貨幣（代幣），均不屬於以下類別：（1）任何種類的貨幣;（b）證券;（C）法律實體的股權;（d）股票，債券，票據，認股權證，證書或其他授予任何權利的文書。

  項目代幣的增值與否取決於市場規律以及應用落地後的需求，EXCUAE團隊不對其增值做出任何承諾，並對其因價值增減所造成的後果概不負責。在適用法律允許的最大範圍內，對因參與交易活動所產生的損害及風險，包括但不限於直接或間接的個人損害，商業盈利的喪失，商業信息的丟失或任何其它經濟損失，EXCUAE團隊不承擔責任EXCUAE平台遵守任何有利於區塊鏈行業健康發展的監管條例以及行業自律申明等參與者將完全接受。參與即代表並遵守此類檢查。同時，參與者披露用以完成此類檢查的所有信息必須完整準確。 DBEX平台明確向參與者傳達了可能的風險，參與者一旦參與平台用戶註冊，代表其已確認理解並認可細則中的各項條款說明，接受EXCUAE平台的潛在風險，後果自擔。

        </pre>
    </li>
              </ul>
            </div>
            <div class='WordSection1' style='layout-grid:15.6pt' v-else>
                <div >Block Chain Group Holding LTD (hereinafter referred to as "the company") is a company operates the website https://www.bcuae.pro.comhereinafter referred to as "this Website" or "the Website"), which is a platform dedicated to the transaction of digital assets and the provision of related services (hereinafter referred to as "the Service"). For the convenience of wording in this Agreement, the Company and the Website are referred to as "we" or other applicable forms of first person pronouns in this Agreement. All-natural persons or other subjects who log onto this Website shall be users of this Website. For the convenience of wording in this Agreement, the users are referred to as "you" or any other applicable forms of the second-person pronouns. For the convenience of wording in this Agreement, you and us are collectively referred to as "both parties", and individually as "one party". 
                </div>
                <em class="paragraph">Important reminder:</em>
                <p> We hereby remind you that:</p>
                <ul>
                  <li>1. The digital assets themselves are not offered by any financial institution, corporation or this Website;</li>
                  <li>2. The digital asset market is new and unconfirmed, and will not necessarily expand;</li>
                  <li>3. Digital assets are primarily used by speculators, and are used relatively less on retail and commercial markets; digital asset transactions are highly risky, due to the fact that they are traded throughout the day without limits on the rise or fall in price, and market makers and global government policies may cause major fluctuations in their prices;</li>
                  <li>4.Digital asset transactions may be suspended or prohibited at any time due to the enactment or modification of national laws, regulations and regulatory documents. Digital assets trading is highly risky and therefore not suitable for the vast majority of people. You acknowledge and understand that investment in digital assets may result in partial or total loss of your investment and therefore you are advised to decide the amount of your investment on the basis of your loss-bearing capacity. You acknowledge and understand that digital assets may generate derivative risks. Therefore, if you have any doubt, you are advised to seek assistance from a financial adviser first. Furthermore, aside from the above-mentioned risks, there may also be unpredictable risks. Therefore, you are advised to carefully consider and use clear judgment to assess your financial position and the abovementioned risks before making any decisions on buying and selling digital assets; any and all losses arising therefrom will be borne by you and we shall not be held liable in any manner whatsoever.
                <p>You are hereby informed that:</p>
                </li>
                </ul>
                <ul>
                  <li>1.You understand that this Website is only intended to serve as a venue for you to obtain digital asset information, find trading counterparties, hold negotiations on and effect transactions of digital assets. This Website does not participate in any of your transactions, and therefore you shall, at your sole discretion, carefully assess the authenticity, legality and validity of relevant digital assets and/or information, and solely bear the responsibilities and losses that may arise therefrom.
                  </li>
                  <li>2. All opinions, information, discussions, analyses, prices, advice and other information on this Website are general market reviews and do not constitute any investment advice. We do not bear any loss arising directly or indirectly from reliance on the abovementioned information, including but not limited to, any loss of profits.</li>
                  <li>3. The content of this Website may be changed from time to time and at any time without notice, and we have taken reasonable measures to ensure the accuracy of the information on the Website; however, we do not guarantee the degree of such accuracy, or bear any loss arising directly or indirectly from the information on this Website or from any delay or failure caused by failure to link up with the internet, transmit or receive any notice and information.
                  </li>
                  <li>4.There are also risks in using internet-based trading systems, including but not limited to the failure of software, hardware and Internet links. Since we cannot control the reliability and availability of the Internet, we are not liable for distortion, delay and failure of the connection.</li>
                  <li>
                      5.	https://www.bcuae.pro.com/ is the sole official external information release platform for this Website;
                  </li>
                  <li>6.This Website do not accept credit card;
                  </li>
                  <li>7.	It is prohibited to use this Website to engage in any illegal transaction activities, such as money laundering, smuggling and commercial bribery. In the event that any of such activities is uncovered, this Website will adopt all available measures, including but not limited to freezing the offender's account, notifying relevant authorities, etc., and we will not assume any of the responsibilities arising therefrom and reserve the right to hold relevant persons accountable. </li>
                  
                </ul>
                <em class="paragraph">1、General Provisions</em>
                <ul>
                  <li>1.1 The User Agreement (hereinafter referred to as "this Agreement" or "these terms and conditions") consists of the main body, Terms of Privacy, Understanding Your client and Anti-money-laundering Policy, as well as any rules, statements, instructions, etc. that this Website has published or may publish in the future.</li>
                  <li>1.2 Before using the services offered by this Website, you shall read this Agreement carefully, and consult a professional lawyer if you have any doubt or as may be otherwise necessary. If you do not agree to the terms and conditions of this Agreement and/or any change made thereto from time to time and at any time, please immediately stop using the service provided by this Website or stop logging onto this Website. Upon your logging into this Website or using any service offered by this Website or engaging in any other similar activity, it shall be deemed as having understood and fully agreeing to all terms and conditions of this Agreement, including any and all changes, modifications or alterations that this Website may make to this Agreement from time to time and at any time.
                  </li>
                  <li>1.3 After filling in the relevant information in accordance with the requirements of this Website, and going through other relevant procedures, you will successfully register yourself as a member of this Website (hereinafter referred to as "Member"); in the process of registration, if you click on the "I Agree", it shall be deemed that you have reached an agreement with the Company by way of electronic signature; or when you use this Website, you click on the "I Agree" button or a similar button, or if you use the services offered by this Website in any of the ways allowed by this Website, it shall be deemed that you fully understand, agree to and accept all the terms and conditions under this Agreement, and in this case, the absence of your handwritten signature will not affect the legal binding force that this Agreement may have on you.
                  </li>
                  <li>1.4 After you become a member of this Website, you will receive a member account and corresponding password, which shall be properly kept by you as a member of this Website; Members shall be liable for all activities and events carried out through their accounts.</li>
                  <li>1.5 You cannot engage in trading on the digital asset trading platform provided by this Website and gain access to the services that are exclusively available to members in accordance with the rules and regulations of this Website, unless and until you become a member of this Website; if you are not a member of this Website, you can only log in to and browse the Website and have access to other services as are permitted by the rules and regulations of this Website.</li>
                  <li>
                    <p>1.6 Upon registering yourself as a member of this Website and using any of the services and functions offered by this Website, it shall be deemed that you have read, understood this Agreement, and:</p>
                    <ul class="indent">
                      <li>1.6.1 accepted to be bound by all terms and conditions of this Agreement;</li>
                      <li>1.6.2 You confirm that you have attained the age of 16, or another statutory age for entering into contracts as is required by a different applicable law, and your registration with this Website, purchase or sale via this Website, release information on this Website and other behaviors indicating your acceptance of the Services offered by this Website shall comply with the relevant laws and regulations of the sovereign state or region that has jurisdiction over you, and you confirm that you have sufficient capacity to accept these terms and conditions, enter into transactions and to use this Website for digital asset transactions.</li>
                      <li>1.6.3 You undertake that all your digital assets involved in transactions hereunder are legally acquired and owned by you.</li>
                      <li>1.6.4 You agree to undertake any and all liabilities for your own transaction and non-transaction activities as well as any and all profits and losses therefrom.</li>
                      <li>1.6.5 You confirm that the information provided at the time of registration is true and accurate.</li>
                      <li>1.6.6 You agree to comply with any and all relevant laws, including the reporting of any transaction profits for tax purposes.</li>
                      <li>1.6.7 This Agreement is only binding on the rights and obligations between you and us, and does not involve legal relations and legal disputes arising from and relating to the transaction of digital assets between the users of this Website, and between other websites and you.</li>
                    </ul>
                  </li>
                </ul>
                <em class="paragraph">2、Revision of the agreemen</em>
                <div>
                2. Amendment of this Agreement We reserve the right to amend this Agreement from time to time, and disclose such amendment by way of announcement on the Website without sending a separate notice to you on your rights. The date when the amendment is made will be indicated on the first page of the amended agreement. The amended agreement will take effect immediately upon announcement on the Website. You shall browse this Website from time to time and follow information on the time and content of amendments, if any, made to this Agreement. If you do not agree with the amendments, you shall stop using the services offered by this Website immediately; if you continue to use the services offered by this Website, it shall be deemed that you accept and agree to be bound by the amended agreement.
                </div>
                <em class="paragraph">3、Registration</em>
                <ul>
                  <!-- <li>3.1 注册资格</li> -->
                  <li>
                  <p>3.1. Eligibility for Registration </p>
                  You confirm and promise that: you shall be a natural person, legal person or other organization with the ability to sign this Agreement and the ability to use the services of this Website, as is provided by applicable laws, when you complete the registration process or when you use the services offered by this Website in any other manner as is otherwise permitted by this Website. Upon clicking on the button indicating that you agree to register, it shall be deemed that you yourself or your authorized agent agrees to the content of this Agreement and your authorized agent will register with this Website and use the services offered by this Website on your behalf. If you are not a natural person, legal person or organization with the abovementioned ability, you and your authorized agent shall bear all the consequences of that, and the company reserves the right to cancel or permanently freeze your account and to hold you and your authorized agent accountable.
                  </li>
                  <!-- <li>3.2 注册目的</li> -->
                  <p> 3.2 Purpose of Registration </p>
                  <li> You confirm and promise that you do not register with this Website for the purpose of violating any of the applicable laws or regulations or undermining the order of digital asset transactions on this Website.</li>
                  <li>
                    <p>3.3 Registration Process</p>
                    <ul class="indent">
                      <li>3.3.1 You agree to provide a valid email address, a mobile phone number and other information in accordance with the requirements on the user registration page of this Website. You can use the email address, mobile phone number or any other manner permitted by this Website to log in to this Website. Where it is necessary and in accordance with the requirements of applicable laws and regulations of relevant jurisdictions, you shall provide your real name, identity card and other information required by applicable laws, regulations, the Terms of Privacy, and anti-money-laundering terms, and constantly update your registration data so that they will be timely, detailed and accurate as is required. All of the original typed data will be referenced as registration information. You shall be responsible for the authenticity, integrity and accuracy of such information and bear any direct or indirect loss and adverse consequences arising out of it.
                      </li>
                      <li>3.3.2 If any of the applicable laws, regulations, rules, orders and other regulatory documents of the sovereign country or region in which you are based requires that mobile phone accounts must be based on real names, you hereby confirm that the mobile phone number you provide for registration purposes has gone through the real-name registration procedure. If you cannot provide such a mobile phone number as is required, any direct or indirect losses and adverse consequences arising therefrom and affecting you shall be borne by you.
                      </li>
                      <li>3.3.3 After you provide the required registration information in a legal, complete and valid manner and such information passes relevant verification, you shall have the right to obtain an account and a password of this Website. Upon obtaining such account and password, your registration shall be deemed as successful and you can log into this Website as a member thereof.</li>
                      <li>3.3.4 You agree to receive emails and/or short messages sent by this Website related to the management and operation thereof.</li>
                    
                    </ul>
                  </li>
                </ul>
                <em class="paragraph">4、Services</em>
                <div>This Website only provides online transaction platform services for you to engage in digital asset trading activities through this Website (including but not limited to the digital asset transactions etc.). This Website does not participate in the transaction of digital assets as a buyer or seller; This Website does not provide any services relating to the replenishment and withdrawal of the legal currency of any country.</div>
                <ul>
                  <li>
                    <p>4.1 Content of Services</p>
                    <ul class="indent">
                      <li>4.1.1 You have the right to browse the real-time quotes and transaction information of digital asset products on this Website, to submit digital asset transaction instructions and to complete the digital asset transaction through this Website.</li>
                      <li>4.1.2 You have the right to view information under the member accounts on this Website and to apply the functions provided by this Website.</li>
                      <li>4.1.3 You have the right to participate in the website activities organized by this Website in accordance with the rules of activities posted on this Website.</li>
                      <li>4.1.4 Other services that this Website promises to offer to you.</li>
                    </ul>
                  </li>
                  <li>
                    <p>4.2 Service </p>
                      &emsp; Rules You undertake to comply with the following service rules of this Website:
                    <!-- <p>您承诺遵守下列本网站服务规则：</p> -->
                    <ul class="indent">
                      <li>4.2.1 You shall comply with the provisions of applicable laws, regulations, rules, and policy requirements, and ensure the legality of the source of all digital assets in your account, and shall refrain from engaging in any illegal activities or other activities that damages the rights and interests of this Website or any third party, such as sending or receiving information that is illegal, illicit or infringes on the rights and interests of any other person, sending or receiving pyramid scheme information or information or remarks causing other harms, unauthorized use or falsification of the email header information of this Website, inter alia.
                      </li>
                      <li>4.2.2 You shall comply with applicable laws and regulations and properly use and keep your account in this Website and login password, password of your financial transactions, and the mobile phone number bound with your account that you provide upon registration of your account, as well as the security of the verification codes received via your mobile phone. You shall be solely responsible for any and all your operations carried out using your account with this Website and login password, financial transaction password, verification codes sent to your mobile phone, as well as all consequences of such operations. When you find that your account with this Website, your login password, financial transaction password, or mobile phone verification codes is used by any unauthorized third party, uncover any other problem relating to the security of your account, you shall inform this Website in a prompt and effective manner, and request this Website to temporarily suspend the services to your account with this Website. This Website shall have the right to take action on your request within a reasonable time; nonetheless, this Website does not bear any liability for the consequences that have arisen before such action is taken, including but not limited to any loss that you may sustain. You may not assign your account with this Website to any other person by way of donation, lending, leasing, transfer or otherwise without the consent of this Website.
                      </li>
                      <li>4.2.3 You agree to take responsibility for all activities (including but not limited to information disclosure, information release, online click-approving or submission of various agreements on rules, online renewal of agreements or purchase service) using your account and password with this Website.</li>
                      <li>4.2.4 In your digital asset transactions on this Website, you may not maliciously interfere with the normal proceeding of the digital asset transaction or disrupt the transaction order; you may not use any technical means or other means to interfere with the normal operation of this Website or interfere with the other users' use of the services; you may not maliciously defame the business goodwill of this Website on the ground of falsified fact.
                      </li>
                      <li>4.2.5 If any dispute arises between you and any other user in connection with online transaction, you may not resort to any means other than judicial or governmental means to request this Website to provide relevant information.</li>
                      <li>4.2.6 All taxes payable as well as all fees relating to hardware, software and services that are incurred by you in the course of using the services provided by this Website shall be solely borne by you.</li>
                      <li>4.2.7 You shall abide by this Agreement and other terms of service and operating rules that this Website may release from time to time, and you have the right to terminate your use of the services provided by this Website at any time.</li>
                    </ul>
                  </li>
                  <li><p>4.3 Product Rules</p>
                    <ul class="indent">
                      <li><p>4.3.1 Rules for trading products</p>
                        <p>You undertake that in the process in which you log into this Website and engage in transactions with other users through this Website, you will properly comply with the following transaction rules.</p>
                        <ul class="indent">
                          <li>4.3.1.1 Browsing transaction information</li>
                          <li>When you browse the transaction information on this Website, you should carefully read all the content in the transaction information, including but not limited to the price, consignment, handling fee, buying or selling direction, and you shall accept all the contents contained in the transaction information before you may click on the button to proceed with the transaction.</li>
                          <li>4.3.1.2 Submission of Commission</li>
                          <li>After browsing and verifying the transaction information, you may submit your transaction commissions. After you submit the transaction commission, it shall be deemed that you authorize this Website to broker you for the corresponding transactions, and this Website will automatically complete the matchmaking operation when there is a transaction proposal that meets your price quotation, without prior notice to you.</li>
                          <li>4.3.1.3 Accessing transaction details</li>
                          <li>You can check the corresponding transaction records in the transaction statements by the Management Center, and confirm your own detailed transaction records.</li>
                          <li>4.3.1.4 Revoking/modifying transaction commission. You have the right to revoke or modify your transaction commission at any time before the transaction is concluded.</li>
                        </ul>
                      </li>
                    </ul>
                  </li>
                </ul>
                <em class="paragraph">5、Rights and Obligations of this Website</em>
                <ul>
                  <li>5.1 If you do not have the registration qualifications agreed on in this Agreement, this Website shall have the right to refuse to allow you to register; if you have already registered, this Website shall have the right to revoke your member account, and this Website reserves the right to hold you or your authorized agent accountable. Furthermore, this Website reserves the right to decide whether to accept your application for registration under any other circumstances.
                  </li>
                  <li>5.2 When this Website finds out that the user of an Account is not the initial registrant of that Account, it shall have the right to suspend or terminate the user's access to that Account.</li>
                  <li>5.3 Where by means of technical testing or manual sampling, among others, this Website reasonably suspects that the information you provide is wrong, untrue, invalid or incomplete, this Website shall have the right to notify you to correct or update the information, or suspend or terminate its supply of the services to you.</li>
                  <li>5.4 This Website shall have the right to correct any information displayed on this Website when it uncovers any obvious error in such information.</li>
                  <li>5.5 This Website reserves the right to modify, suspend or terminate the Services offered by this Website, at any time, and the right to modify or suspend the Service without prior notice to you; if this Website terminates one or more of the Services offered by this Website, such termination by this Website will take effect on the date of announcement of such termination on the Website.</li>
                  <li>5.6  This Website will take necessary technical methods and management surveillance to ensure the daily operation of this Website and shall maintain the order of digital assets trading by providing a necessary and reliable transaction services. </li>
                  <li>5.7 If you fail to log into this Website using your member account number and password for an uninterrupted period of one year, this Website shall have the right to revoke your account. After your account is revoked, this Website shall have the right to offer the member name represented by such account to other applicants for membership.</li>
                  <li>5.8 This Website shall ensure the security of your digital assets by strengthening technical input and enhancing security precautions, and is under the obligation to notify you in advance of the foreseeable security risks in your account.</li>
                  <li>5.9 This Website shall have the right to delete all kinds of content and information which does not conform to laws and regulations or the rules of this Website at any time, and exercise of this right by this Website is not subject to a prior notice to you.</li>
                  <li>5.10 This Website shall have the right to, in accordance with the applicable laws, administrative regulations, rules, orders and other regulatory documents of the sovereign country or region where you are based, request to you for more information or data, and to take reasonable measures to meet the requirements of the local standards, and you have the obligation to provide proper assistance to such measures; this Website shall have the right to suspend or permanently terminate your access to this Website as well as part or all of the services offered by this Website.
                  </li>
                </ul>
                <em class="paragraph">6、Indemnity</em>
                <ul>
                  <li>6.1 Under any circumstance, our liability for your direct damage will not exceed the total cost incurred by your three (3) months' use of services offered by this Website.</li>
                  <li>6.2 Shall you breach this Agreement or any applicable law or administrative regulation, you shall pay to us at least US$ Two million in compensation and bear all the expenses in connection with such breach (including attorney's fees, among others). If such compensation cannot cover the actual loss, you shall make up for the difference.</li>
                </ul>
                <em class="paragraph">7、The Right to Injunctive Relief </em>
                <div>Both you and we acknowledge that common law remedies for breach of agreement or possible breach of contract may be insufficient to cover all the losses that we sustain; therefore, in the event of a breach of contract or a possible breach of contract, the non-breaching party shall have the right to seek injunctive relief as well as all other remedies that are permitted under common law or equity.</div>
                <em class="paragraph">8、Limitation and Exemption of Liability</em>
                <ul>
                  <li><p>8.1 You understand and agree that under no circumstance will we be held liable for any of the following events:</p>
                    <ul class="indent">
                      <li>8.1.1 loss of income;</li>
                      <li>8.1.2 loss of transaction profits or contractual losses;</li>
                      <li>8.1.3 disruption of the business</li>
                      <li>8.1.4 loss of expected currency losses</li>
                      <li>8.1.5 loss of information</li>
                      <li>8.1.6 loss of opportunity, damage to goodwill or reputation</li>
                      <li>8.1.7 damage or loss of data;</li>
                      <li>8.1.8 cost of purchasing alternative products or services;</li>
                      <li>8.1.9 any indirect, special or incidental loss or damage arising from any infringement (including negligence), breach of contract or any other cause, regardless of whether or not such loss or damage may reasonably be foreseen by us, and regardless of whether or not we are notified in advance of the possibility of such loss or damage.</li>
                      <li>8.1.10 Items 8.1.1 to 8.1.9 are independent of each other.</li>
                    </ul>
                  </li>
                  <li><p>8.2 You understand and agree that we shall not be held liable for any damages caused by any of the following events:</p>
                    <ul class="indent">
                      <li>8.2.1 Where we are properly justified in believing that your specific transactions may involve any serious violation or breach of law or agreement;</li>
                      <li>8.2.2 Where we are reasonably justified in believing that your conduct on this Website is suspected of being illegal or immoral;</li>
                      <li>8.2.3 The expenses and losses arising from the purchase or acquisition of any data, information or transaction, etc. through the services offered by this Website;</li>
                      <li>8.2.4 Your misunderstanding of the Services offered by this Website;</li>
                      <li>8.2.5 Any other losses related to the services provided by this Website, which cannot be attributed to us.</li>
                    </ul>
                  </li>
                  <li>8.3 Where we fail to provide the Services or delay in providing such Services due to information network equipment maintenance, information network connectivity failures, errors in computer, communications or other systems, power failures, weather conditions, unexpected accidents, industrial actions, labor disputes, revolts, uprisings, riots, lack of productivity or production materials, fires, floods, storms, explosions, wars, failure on the part of banks or other partners, collapse of the digital asset market, actions by government, judicial or administrative authorities, other acts that are not within our control or beyond our inability to control, or due to causes on the part of third parties, we shall not assume any responsibility for such failure to provide service or delay in providing services, or for the resultant loss you may sustain as a result of such failure or delay.
                  </li>
                  <li>8.4 We cannot guarantee that all the information, programs, texts, etc. contained in this Website are completely safe, free from the interference and destruction by any malicious programs such as viruses, trojans, etc., therefore, your log-into this Website or use of any services offered by this Website, download of any program, information and data from this Website and your use thereof are your personal decisions and therefore you shall bear the any and all risks and losses that may possibly arise.
                  </li>
                  <li>8.5 We do not make any warranties and commitments in connection with any of the information, products and business of any third party websites linked to this Website, as well as any other forms of content that do not belong to us; your use any of the services, information, and products provided by a third party website is your personal decision and therefore you shall assume any and all the responsibilities arising therefrom.
                  </li>
                  <li>8.6  We do not make any explicit or implicit warranties regarding your use of the Services offered by this Website, including but not limited to the applicability, freedom from error or omission, consistency, accuracy, reliability, and applicability to a specific purpose, of the services provided by this Website. Furthermore, we do not make any commitment or guarantee in connection with the validity, accuracy, correctness, reliability, quality, stability, integrity and timeliness of the technology and information covered by the services offered by this Website. Whether to log in this Website or use the services provided by this Website is your personal decision and therefore you shall bear all the risks and possible losses arising from such decision. We do not make any explicit or implicit warranties in connection with the market, value and price of digital assets; you understand and acknowledge that the digital asset market is unstable, that the price and value of assets may fluctuate or collapse at any time, and that the transaction of digital assets is based on your personal free will and decision and therefore you shall assume any and all risks and losses that may possible arise therefrom.
                  </li>
                  <li>8.7 The guarantees and undertakings specified in this Agreement shall be the only guarantee and statements that we make in connection with the Services provided by us under this Agreement and through this Website, and shall supersede any and all the warranties and commitments arising in any other way and manner, whether in writing or in words, express or implied. All these guarantees and statements represent only our own commitments and undertakings and do not guarantee any third party's compliance with the guarantees and commitments contained in this Agreement.
                  </li>
                  <li>8.8 We do not waive any of the rights not mentioned in this Agreement and to the maximum extent permitted by the applicable law, to limit, exempt or offset our liability for damages.</li>
                  <li>8.9 Upon your registration of your account with this Website, it shall be deemed that you approve any and all operations performed by us in accordance with the rules set forth in this Agreement, and any and all risks arising from such operations shall be assumed by you.</li>
                </ul>
                <em class="paragraph">9、Termination of Agreement</em>
                <ul>
                  <li>9.1 This Website shall have the right to cancel your account with this Website in accordance with this Agreement, and this Agreement shall be terminated on the date of the cancellation of your account.</li>
                  <li>9.2 This Website shall have the right to terminate all Service offered by this Website to you in accordance with this Agreement, and this Agreement shall terminate on the date of termination of all services offered by this Website to you.</li>
                  <li>9.3 After the termination of this Agreement, you do not have the right to require this Website to continue to provide you with any service or perform any other obligation, including, but not limited to, requesting this Website to keep or disclose to you any information in your former original account, or to forward to you or any third party any information therein that is not read or sent.</li>
                  <li>9.4 The termination of this Agreement shall not prevent the observant party from demanding the breaching party to assume other liabilities.</li>
                </ul>
                <em class="paragraph">10、Intellectual Property</em>
                <ul>
                  <li>10.1 All intellectual achievements included in this Website, including, but not limited to, website logos, databases, website design, text and graphics, software, photos, videos, music, sounds and any combinations of the aforementioned files, and the intellectual property rights of software compilation, associated source code and software (including small applications and scripts) shall be owned by this Website. You may not copy, modify, copy, transmit or use any of the foregoing materials or content for commercial purposes.
                  </li>
                  <li>10.2 All rights contained in the name of this Website (including but not limited to business goodwill and trademarks, logos) shall be owned by the Company.</li>
                  <li>10.3 Upon accepting this Agreement, it shall be deemed that you, on the basis of your own free will, have transferred and assigned exclusively and free of charge to this Website all copyright of any form of information that you publish on this Website, including, but not limited to copyrights, distribution rights, lease rights, exhibition rights, performance rights, projection rights, broadcasting rights, information network dissemination rights, shooting rights, adaptation rights, translation rights, compilation rights and other transferable rights that copyright owners are entitled to, and this Website shall have the right to sue for any infringement on such copyright and obtain full compensation for such infringement. This Agreement shall apply to any content that is published by you on this Website and is protected by copyright law, regardless of whether the content is generated before or after the signing of this Agreement.
                  </li>
                  <li>10.4 You shall not illegally use or dispose of the intellectual property rights of this Website or any other person during your use of the services offered by this Website. For any information that you publish on this Website, you may not publish or authorize other websites (or media) to use such information in any manner whatsoever.</li>
                  <li>10.5 Your log into this Website or use of any of the services offered by this Website shall not be deemed as our transfer of any intellectual property to you.</li>
                </ul>
                <em class="paragraph">11、Information protection</em>
                <ul>
                  <li><p>11.1. Scope of Application</p>
                    <ul class="indent">
                      <li>11.1.1 When you register your account with this Website or use your account with this Website, you shall provide personal registration information in accordance with the requirements of this Website, including but not limited to your telephone number, email address, and identity card information.</li>
                      <li>11.1.2 When you use the services offered by this Website, or visit this Website, this Website will automatically receive and record the server information of your web browser, including but not limited to the IP address and records on the web pages that you request to access.</li>
                      <li>11.1.3 The relevant data collected by this Website in connection with your transactions on this Website, including but not limited to transaction records.</li>
                      <li>11.1.4 Other personal information of yours legally obtained by this Website.</li>
                    </ul>
                  </li>
                  <li><p>11.2 Use of Information </p>
                    <ul class="indent">
                      <li><p>11.2.1 Upon your successful registration with this Website and without extra consent from you, it shall be deemed that you agree to permit this Website to collect and use all the information you publish on this Website; as is specified under 11.1 hereof, you acknowledge and agree that this Website can use your information collected by this Website for certain purposes, including but not limited to the following: </p>
                        <ul class="indent">
                          <li>11.2.1.1 providing you with the services offered by this Website;</li>
                          <li>11.2.1.2 Reporting to relevant regulatory departments based on the requirements of the competent authorities in relevant sovereign states or regions;</li>
                          <li>11.2.1.3 When you use Services offered by this Website, this Website will use your information for such legal purposes as identity authentication, customer service, security, fraud monitoring, marketing & promotion, archiving, and backup, or joint promotion of this Website with a third party, so as to ensure the security of the products and services that this Website offers to you;</li>
                          <li>11.2.1.4 Information collection and processing for the purpose of helping this Website design new products and services and improving the existing services offered by this Website;</li>
                          <li>11.2.1.5 In order to enable you to understand the specifics of the Services offered by this Website, you agree to permit this Website to send to you marketing event information, commercial electronic information, and advertising that is related to you in replacement of general-purpose ubiquitous advertising;</li>
                          <li>11.2.1.6 This Website may transfer or disclose your information to any third party that is not a related party of this Website, for the purpose of completing merger, division, acquisition or transfer of assets;</li>
                          <li>11.2.1.7 Software certification or management software upgrade;</li>
                          <li>11.2.1.8 Inviting you to participate in surveys in connection with the services offered by this Website;</li>
                          <li>11.2.1.9 Data analysis relating to cooperation with government agencies, public affairs agencies, associations, etc;</li>
                          <li>11.2.1.10 For all other legal purposes as well as other purposes authorized by you.</li>
                        </ul>
                      </li>
                      <li>11.2.2 This Website will not sell or lend your personal information to any other person unless your permission is obtained in advance. This Website also does not allow any third party to collect, edit, sell or gratuitously spread your personal information in any manner whatsoever.</li>
                    </ul>
                  </li>
                  <li>11.3 This Website shall keep confidential the customer identity information and transaction information that it obtains, and shall not provide any entity or individual with customer identification information or transaction information, except where any of the applicable laws, regulations, decrees, orders, etc., of relevant sovereign states or regions requires this Website to provide such information.</li>
                </ul>
                <em class="paragraph">12、Calculation</em>
                <p>All the transaction calculations are verified by us, and all the calculation methods have been posted on the Website, but we can not ensure that your use of this Website will not be disturbed or free from errors. </p>
                <em class="paragraph">13、Export Control</em>
                <p>You understand and acknowledge that in accordance with relevant laws of The United Arab Emirates, you shall not export, re-export, import or transfer any material (including software) on this Website; therefore, you hereby undertake that you will not voluntarily commit or assist or participate in any of the above export or related transfer or other violations of applicable laws and regulations; if you uncover any of.</p>
                <em class="paragraph">14、Transfer</em>
                <p>the rights and obligations agreed in this Agreement shall be equally binding on the assignees, the heirs, executors and administrators of the parties hereto who benefit from the rights and obligations. Without our consent, you may not transfer to any third party any of your rights or obligations hereunder, provided, however, we may, at any time, assign our rights and obligations under this Agreement to any third party with thirty (30) days' notice to you.</p>
                <em class="paragraph">15、Severability</em>
                <p>if any provision of this Agreement is found unenforceable, invalid or illegal by any court of competent jurisdiction, validity of the remaining provisions of this Agreement shall not be affected.</p>
                <em class="paragraph">16、No Agency</em>
                <p>Nothing in this Agreement shall be deemed to have created, implied or otherwise treated us as your agent, trustee or other representative, unless it is provided otherwise in this Agreement.</p>
                <em class="paragraph">17、Waiver</em>
                <p>Our or your waiver of the right to hold the other party liable for breaches of agreement or any other liability as is agreed upon in this Agreement shall not be construed or deemed as a waiver of the right to hold the other party for other breaches of contract; a failure to exercise any right or remedy shall not be construed in any way as a waiver of such right or remedy. </p>
                <em class="paragraph">18、Headings</em>
                <p>All headings herein are exclusively for the convenience of wording and are not intended to expand or limit the content or scope of the terms and conditions of this Agreement.</p>
                <em class="paragraph"> 19、Applicable Law</em>
                <p>This Agreement in its entirety is a contract concluded under the laws of the Republic of Singapore, and relevant laws of the Republic of Singapore shall apply to its establishment, interpretation, content and enforcement; Any claims or actions arising out of or relating to the Services agreed in this Agreement shall be governed and interpreted and enforced in accordance with the laws of the Republic of Singapore. For the avoidance of doubt, this Clause shall be expressly applicable to any tort claim against us. The competent court or forum for any claim or action against us or in relation to us shall be in the Republic of Singapore. You have unconditional access to exclusive jurisdiction in court proceedings and appeals in the courts of the Republic of Singapore. You also unconditionally agree that the venue or competent court for any dispute or problem relating to this Agreement or any claim and proceeding arising from this Agreement shall be exclusively in the Republic of Singapore. If any other business of this Website is subject to any special agreement on jurisdiction, such agreement shall prevail. The Doctrine of Forum Non Conveniens does not apply to the court of choice under these Terms of Service.</p>
                <em class="paragraph">20、Entry into Force and Interpretation of the Agreement </em>
                <ul>
                  <li>20.1 This Agreement shall enter into force when you click through the registration page of this Website, complete the registration procedures, obtain your account number and password of this Website, and shall be binding on you and this Website.</li>
                  <li>20.2 The ultimate power of interpretation of this Agreement shall be vested in this Website.</li>
                </ul>
                <em class="paragraph"><span class="large_title"> Know-your-customers and Anti-Money Laundering Policies</span></em> <em class="paragraph">1、Preamble</em>
                <ul>
                  <li>
                    1.1 We ensure that we comply with know-your-customer and anti-money-laundering laws and regulations, and will not knowingly violate know-your-customers and anti-money-laundering policies. To the extent of our reasonable control, we will adopt necessary measures and technology to provide you with Services that are safe and secure, so as to protect you against the loss caused by money laundering to the greatest extent possible.
                  </li>
                  <li>1.2 Our know-your-customer and anti-money-laundering policies are a comprehensive system of international policies, including the know-your-customer and anti-money-laundering policies of the jurisdictions to which you are subject to. Our robust compliance framework ensures that we meet regulatory requirements and regulatory standards on both the local and global levels, and ensure the operational sustainability of our website.
                  </li>
                </ul>
                <em class="paragraph">2、Content of Our Know-Your-Customer and Anti-Money-Laundering Policies</em>
                <ul>
                  <li>2.1 We promulgate and update know-your-customers and anti-money-laundering policies to meet the standards set by relevant laws and regulations;</li>
                  <li>2.2 We promulgate and update some of the guidelines and rules in connection with the operation of this Website, and our staff will provide you whole-process service in accordance with the guidelines and rules;</li>
                  <li>2.3 We design and complete the procedures for internal monitoring and transaction control, such as rigorous identity authentication procedures, and form a professional team responsible for anti-money laundering;</li>
                  <li>2.4 We adopt risk-prevention-based approach to carry out due diligence and continuous supervision in connection with customers;</li>
                  <li>2.5 Review and regularly inspect existing transactions;</li>
                  <li>2.6 To report suspicious transactions to the competent authorities;</li>
                  <li>2.7 Proof documents of identity documents, address certificates and transaction records will be maintained for at least six(6) years; if they are submitted to the regulatory authorities, let it be understood that a separate notice will not be provided to you;</li>
                  <li>2.8 Credit cards are prohibited throughout the course of the transaction;</li>
                </ul>
                <em class="paragraph">3、Identity Information and the Verification and Confirmation Thereof </em>
                <ul>
                  <li><p>3.1 Identity Information</p>
                    <ul class="indent">
                      <li>3.1.1 In accordance with the laws and regulations of relevant jurisdictions and in light of the nature of entities concerned, the content of your information as is collected by us may vary, and in principle, we will collect the following information of yours if you register as an individual: Basic personal information: your name, address (and permanent address, if the two are different), date of birth and nationality, and other information available. Identity authentication shall be based on documents issued by the official or other similar authorities, such as passports, identity cards or other identity documents as are required and issued by relevant jurisdictions. The address you provide will be validated in an appropriate manner, such as checking the fare ticket of means of transportation you use, your interest rate bills, or voter register. Valid photo: before you register, you must provide a photograph showing you holding your identity document in front of your chest; Contact information: telephone/mobile phone number and valid email address.
                      </li>
                      <!-- <li>有效的照片：在您注册之前，您须提供您将您的身份证件放在胸前的照片；</li>
                      <li>联系方式：电话/手机号码和/或有效的电子邮件地址。</li> -->
                      <li>3.1.2 If you are a company or any other type of legal entity, we will collect the following information of yours to determine the final beneficiary of your account or your trust account. Your corporation enrollment and registration certificates of the company; a copy of the articles of association and memorandum of the company; the detailed certification materials of the ownership structure and ownership description of the company, and the decision of the board of directors on designating the authorized agent of the company responsible for the opening and execution of the account of the company with the website; the identity documents of the directors, major shareholders of the company as well as the authorized signatory for the company's account with the website, as are required to be provided in accordance with relevant rules; the company's main business address, and the company's mailing address if it is different from the main business address of the company. If the local address of the company is different from its main business address, the company shall be deemed to be a high-risk customer, and consequently the company will be required to provide additional documentation. Other certification documents, documents issued by competent authorities and other documents we may deem necessary in light of the laws and regulations of relevant jurisdictions and in light of the specific nature of your entity.</li>
                      <!-- <li>
                        公司注册、登记证；公司的章程与备忘录副本；公司的股权机构和所有权说明的详细证明材料，证明决定本网站账户的开立以及执行的授权委托人的董事会决议；按照要求需要提供的公司董事、大股东及本网站账户有权签字人的身份证明文件；该公司的主要营业地址，如果与公司的邮寄地址不同，提供邮寄地址。如果公司在本地的地址与它的主要营业地址不一致的，则被视为风险较高的客户，需要提交额外附加文件。
                      </li>
                      <li>•根据不同的司法管辖区的不同规定及不同的实体类型，我们要求的其他认证和权威部门发布的文件以及我们认为必要的文件。</li> -->
                      <li>3.1.3 We only accept English and Chinese versions of your identity information; if your identity information is not in either of the two languages, you shall have your identity information translated into English and duly notarized.</li>
                    </ul>
                  </li>
                  <li><p>3.2 Confirmation and Verification</p>
                    <ul class="indent">
                      <li>3.2.1 You are required to provide both the front and back sides of your identity documents.</li>
                      <li>3.2.2 You are required to provide us with a photograph showing you holding your identity documents in front of your chest.</li>
                      <li>3.2.3 Copies of certification documents shall be checked against the originals thereof. Nonetheless, if a trusted and suitable certifier person can prove that such copies are accurate and comprehensive duplicates of the originals thereof, such copies shall be deemed as acceptable. Such certifiers include ambassadors, members of the judiciary, magistrates, etc.</li>
                      <li>3.2.4 The identification the ultimate beneficiary and controller of the account shall be based on the determination of which individuals ultimately own or control the direct customer and/or to determining that the ongoing transaction is performed by another person. If you are a business enterprise, the identity of major shareholders thereof (for example, those holding 10 % or more of the voting equity in such business enterprise) shall be verified. Generally, a shareholder holding 25 % of the shares of the company will be deemed as involving an average level of risk, and the identity of the shareholder shall be verified; a shareholder holding 10 % or more of the voting rights or shares is deemed to be involving a high level of risk, and the identity of the shareholder shall be verified.
                      </li>
                    </ul>
                  </li>
                </ul>
                <em class="paragraph">4、Transaction Supervision</em>
                <ul>
                  <li>4.1 We constantly set and adjust daily trading and cash withdrawal limits based on security requirement and actual state of transactions;</li>
                  <li>4.2 If the transaction occurs frequently in an account registered by you or is beyond reasonable circumstances, our professional team will assess and determine whether such transaction is suspicious;</li>
                  <li>4.3 If we identify a specific transaction as suspicious on the basis of our assessment, we may adopt such restrictive measures as suspending the transaction or denying the transaction, and if it is possible, we may even reverse the transaction as soon as possible, and report to the competent authorities, without, however, notifying you;</li>
                  <li>4.4 We reserve the right to reject registration applications by applicants that do not comply with the international standards against money laundering or who may be regarded as political and public figures; we reserve the right to suspend or terminate a transaction identified as suspicious based on our own assessment, which, however, does not breach any of our obligations and duties to you.</li>
                </ul>
            </div>
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
  color: #d58c2a;
  font-weight: bold;
  border-bottom: 2px solid #d58c2a;
}

/*.content {*/
/*width: 1200px;*/
/*margin: 0 auto;*/
/*font-size: 14px;*/
/*}*/
/*.content div,*/
/*.content p.paragraph{*/
/*text-indent: 2em;*/
/*}*/
/*.content .paragraph {*/
/*font-weight:  bold;*/
/*}*/
/*.content ul {*/
/*margin-bottom: 10px;*/
/*}*/
/*h2 {*/
/*text-align: center;*/
/*}*/

.content {
  padding-top: 20px;
  /*padding-left: 200px;*/
  padding-bottom: 20px;
  text-align: left;
  padding-left: 20px;
  padding-right: 20px;
  background-color: #222327;
}

.content .ivu-col {
  text-align: left;
}

.content p {
  
  margin-bottom: 10px;
  font-size: 14px;
}
.content > div {
  padding-bottom: 20px;
}
.content {
  text-indent: 2em;
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
  font-size: 16px;
  line-height: 22px;
}
.WordSection1 li{
  margin-bottom: 20px;
}
.WordSection1 em{
  line-height: 30px;
  font-weight: 600;
  margin-bottom: 10px;
  display: block;
  font-style: normal;
}
</style>
<script>
export default {
  components: {},

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
