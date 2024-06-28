<script>
  let menu = "";
  function handleMenuButton() {
    if (menu.style.display === "block") {
      menu.style.display = "none";
    } else {
      menu.style.display = "block";
    }
  }
</script>

<div class="container">
  <header>
    <div class="header-container">
      <div class="logo">
        <a href="/">
          <h1>부천노래방</h1>
        </a>
      </div>
      <div class="menu">
        <ul>
          <li><a href="#about">소개</a></li>
          <li><a href="#price">가격</a></li>
          <li><a href="#alba">알바</a></li>
          <li><a href="#contact">문의</a></li>
        </ul>
      </div>
      <div class="mc-container">
        <button on:click={handleMenuButton} class="mc-menu-button">
          <div></div>
          <div></div>
          <div></div>
        </button>
        <nav class="mc-menu" bind:this={menu}>
          <ul>
            <li><a href="#about">소개</a></li>
            <li><a href="#price">가격</a></li>
            <li><a href="#alba">알바</a></li>
            <li><a href="#contact">문의</a></li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
  <main>
    <!-- 소개 -->
    <section id="about">
      <div class="section-container">
        <div class="item">
          <img src="/logo1.gif" loading="lazy" alt="부천역노래방, 부천노래방" />
        </div>
        <div class="item">
          <h2>부천노래방 소개</h2>
          <h3>무한초이스</h3>
          <h3>마인드 싸이즈 최고</h3>
          <h3>픽업서비스</h3>
          <p>
            퍼블릭은 대중적인 가라오케를 일컫는 용어로, 쩜오, 텐카페보다 저렴한
            주대로 로테이션 방식이 아닌 지정 아가씨를 초이스하여 착석하는
            방식으로 진행되고 있다. 단, 초이스 후에 소위 인사시스템은 없으며,
            분위기 있는 술자리를 하는 곳이라고 생각하면 된다.
          </p>
        </div>
      </div>
    </section>

    <!-- 가격 -->
    <section id="price">
      <div class="section-container">
        <div class="item">
          <h2>부천노래방 가격</h2>
          <h3>술,안주 무한제공</h3>
          <h3>TC포함 추가금없음</h3>
          <p>
            퍼블릭 룸카페는 요즘들어 많이 유행하고 있는 룸카페로 "노래방 대신
            퍼블릭으로" 라는 말이 생겨날 정도로 일반적인 룸카페 종류이다.
            퍼블릭은 일반적으로 가장 널리 알려져 있는 룸살롱으로 주대가 저렴해
            비즈니스맨들의 발길이 끊이지 않는 곳이다.
          </p>
        </div>
        <div class="item">
          <img
            src="/logo2.gif"
            loading="lazy"
            alt="부천역노래방가격, 부천노래방가격"
          />
        </div>
      </div>
    </section>

    <!-- 알바 -->
    <section id="alba">
      <div class="section-container">
        <div class="item">
          <img
            src="/logo3.gif"
            loading="lazy"
            alt="부천역노래방알바, 부천노래방알바"
          />
        </div>
        <div class="item">
          <h2>부천노래방 알바</h2>
          <h3>일많음</h3>
          <h3>업계최고대우</h3>
          <h3>출퇴근지원</h3>
          <p>
            유흥주점(룸살롱)과의 차이점은, 유흥업소는 유흥 종사자를 둘 수 있고
            댄스 플로어를 설치하여 춤을 추는 행위가 허용되지만, 단란주점은
            노래방기기를 사용하여 노래를 부르는 정도까지만 허용이 된다는 점이다.
            그러므로 법적으로 단란주점에는 접객을 위한 종업원을 둘 수 없으며,
            식당처럼 주류와 음식을 판매하면서, 노래방처럼 노래를 부를 수 있는
            룸이 있는 형태를 가진다. 그래도 대개 유흥주점으로 분류된다.
          </p>
        </div>
      </div>
    </section>

    <!-- 문의 -->
    <section id="contact">
      <div class="section-container">
        <div class="item">
          <h2>문의하기</h2>
          <p>언제든 편하게 문의주세요</p>
          <address>
            <p>010-9922-5375</p>
            <a href="tel:0109922-5375">
              <button>바로연결</button>
            </a>
          </address>
          <p>친절상담</p>
        </div>
        <div class="item">
          <div class="video-container">
            <iframe
              width="560"
              height="315"
              src="https://www.youtube.com/embed/hokT0QBGfgc?si=X86XntEpkc4A4uWW"
              title="YouTube video player"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              referrerpolicy="strict-origin-when-cross-origin"
              allowfullscreen
            ></iframe>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <nav>
      <div class="menu">
        <ul>
          <li><a href="#about">소개</a></li>
          <li><a href="#price">가격</a></li>
          <li><a href="#alba">알바</a></li>
          <li><a href="#contact">문의</a></li>
        </ul>
      </div>
    </nav>
  </footer>
</div>

<style>
  /*  */
  .header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  /*  */
  .container {
    max-width: 1000px;
    margin: auto;
  }

  .section-container {
    display: flex;
    flex-wrap: wrap;
  }

  .item {
    width: 100%;
  }
  .item img {
    width: 100%;
  }

  /*  */
  .logo a {
    color: inherit;
    text-decoration: none;
  }

  /*  */
  .menu {
    display: none;
  }

  .menu ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
  }

  .menu ul li {
    padding: 10px;
  }

  /* mc-menu */
  .mc-menu-button {
    top: 15px;
    right: 15px;
    cursor: pointer;
  }

  .mc-menu-button div {
    width: 30px;
    height: 5px;
    background-color: #333;
    margin: 6px 0;
  }

  .mc-menu {
    display: none;
    position: absolute;
    top: 85px;
    right: 0;
    width: 200px;
    background-color: #f1f1f1;
  }

  .mc-menu ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  .mc-menu li a {
    display: block;
    padding: 10px;
    text-decoration: none;
  }

  .video-container {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 비율 */
    overflow: hidden;
  }
  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  /* 큰 사이즈 */
  @media screen and (min-width: 768px) {
    .menu {
      display: block;
    }
    .mc-container {
      display: none;
    }
    .item {
      width: 50%;
    }
  }
</style>
