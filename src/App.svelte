<script>
  import "./style.scss";
  import bgm from "./assets/angel-piano.mp3";
  let starSignCard = document.getElementsByClassName("star-sign-card");
  let audioElement;
  function showCard() {
    for (let i = 0; i < starSignCard.length; i++) {
      starSignCard[i].classList.toggle("active");
    }
  }
  function playMusic() {
    if (audioElement.paused) {
      audioElement.volume = 0.7;
      audioElement.play();
    } else {
      audioElement.pause();
    }
  }
</script>

<button class="music" on:click={playMusic}>&#119070;</button>
<audio bind:this={audioElement} src={bgm} />
<main>
  <button on:click={showCard}>What`s your star sign?</button>
  <div class="star-sign-card">
    <p>
      <span>&#9809;12/22~1/20</span><br />
      非常自律 ，為達目的會堅持不懈 ，謹慎、可靠 、有責任感，對自己有相當的抱負。不熟的人會覺得有一層距離感，無法真的了解他們的內心想法，也因此給人一種什麼事都自己來的感覺，然而只要遇到值得信賴的人，便會坦誠相待。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9810;1/21~2/18</span><br />
      求知慾強、興趣廣泛，樂於嘗試不同的新事物，且創意十足 ，富有改革與冒險家精神
      。 也是大家一致公認的外星人星座，個性古怪 ，很常會陷入自己的小世界，對許多事有獨樹一格的見解，有些人認為水瓶座在工作上很叛逆
      、不合群，且容易心不在焉 。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9811;2/19~3/20</span><br />
      感情豐沛、極富同情心又善解人意，是個標準的浪漫主義者 ，天性溫柔無私且很會察言觀色，然而因為有時太憑感覺做事，想法單純
      ，反而給人不切實際 、軟弱、逃避現實的印象。
    </p>
  </div>

  <div class="star-sign-card">
    <p>
      <span>&#9800;3/21~4/20</span><br />
      生性大方、開朗 ，待人親切，即便是初次見面的陌生人，都能很快地打成一片，且行事風格自由，不喜歡受拘束，具冒險精神
      。然而，有時因過度急躁 ，且無法接受批評，反而會弄巧成拙，建議適時將腳步放慢，多點耐心，在工作或人際相處上都會更順利喔！
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9801;4/21~5/21</span><br />
      個性勤勞 、務實 、穩重，且溫和順從，總是笑臉待人且不管別人閒事，是高明的社交高手，他們很有主見、有耐心及責任感
      ，且具有商業頭腦。但也是出了名的固執，且因他們理性的思考模式，偶爾給人過於冷淡的印象。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9802;5/22~6/21</span><br
      />有敏銳的觀察力，有豐富的靈感與想像力，在人際關係上，給人活潑
      、健談的印象，善於隨機應變與說服別人，是個很好的傾聽者
      ，也會照顧朋友，善於交際。然而也很善變，沒有耐心
      ，有時在一段感情裡會過分猜忌，導致兩人間的出現誤會與摩擦。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9803;6/22~7/22</span><br />
      愛家的最佳代表星座，除了用心對待家人外，更用心對待朋友與另一半，非常重情義與有包容心。他們個性節儉、熱心
      ，也擅於理財。然而因為他們太在乎他人的情緒，有時反而犧牲自己的感受，過於多愁善感
      ，給人一種喜怒無常的印象。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9804;7/23~8/22</span><br />
      總是展現自信的一面，他們具有同情心與幽默感 ，為人熱心 ，且不安於命運的安排，他們會努力改變自己的命運，達到自己的目標。然而有時主觀意識太強，會自視甚高。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9805;8/23~9/22</span><br />
      龜毛、完美主義者 、難以取悅是多數人的印象，但其實這都是注重細節的展現，他們擅長規劃且很有耐心，由於他們頭腦清晰、分析能力強，因此在職場上很值得信任，但有時過於講求完美，反而會讓自己壓力太大。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9806;9/23~10/23</span><br />
      標準的和平愛好者，不喜好衝突與爭執，個性體貼、平易近人 、好相處，非常善於交際
      ，也是理想主義者，重視浪漫氛圍。然而個性游移不定、優柔寡斷 ，很難下決定，因此容易隨波逐流，對事情沒有太多的主見，適時地堅持己見反而可以讓其他人更重視並了解他們的想法。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9807;10/24~11/22</span><br />
      心思敏感且細膩的星座，大家普遍認為忌妒心與報復心都很強，且佔有慾很高，這是因為他們對感情的態度秉持著誠實
      至上的原則，他們不喜歡被欺騙，也因此更敢愛敢恨。有時容易感情用事，心機較深，也會有干涉別人事情的行為發生。
    </p>
  </div>
  <div class="star-sign-card">
    <p>
      <span>&#9808;11/23~12/21</span><br />
      做人坦率 、適應力強 、愛好自由，且極富正義感，在處理事情時極具外交手腕，有很好的判斷力，並善於危機處理，但有時因個性敏感
      或過於浮躁 ，講話心直口快，反而給人行事衝動或不負責任的印象，在工作上要多注意一些，才不會造成誤會。
    </p>
  </div>
</main>
