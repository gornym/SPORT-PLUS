<template>
  <body>
    <header>
      <nav class="nav-pc">
        <ul class="ul-left">
          <li>
            <a href="#">
              <img src="@/assets/ul-left.png" alt="Mój obraz" />
            </a>
          </li>
        </ul>
        <div class="logo-nav">
          <button href="#" @click="scrollToTop">
            <img src="@/assets/logo.png" alt="Mój obraz" />
          </button>
        </div>
        <ul class="ul-right">
          <li>
            <a href="#">
              <img src="@/assets/ul-right.png" alt="Mój obraz" />
            </a>
          </li>
        </ul>
      </nav>
      <div class="header-box">
        <a>
          Zarezerwuj wybrane <br />
          obiekty sportowe w całej Polsce
        </a>
        <div class="header-main-box">
          <div class="header-main-box-left">
            <img src="@/assets/ekrany.png" />
          </div>
          <div class="header-main-box-right">
            <h2>
              Postaw na wygodę i zarezerwuj wybrane miejsce<br />
              nie tracąc swojego cennego czasu. <br /><br />
              W naszej ofercie znajdziesz orliki, korty<br />
              tenisowe, siłownie i wiele więcej. <br /><br />
              Dokładamy wszelkich starań, żeby nasi<br />
              użytkownicy mogli dokonać rezerwacji<br />
              w dowolnym miejscu w kraju.
            </h2>
          </div>
        </div>
        <div class="find-more-iphone">
          <button href="#section1" @click="scrollToSection">
            Dowiedz się więcej
            <img alt="Find more" src="@/assets/bottom.png" />
          </button>
        </div>
      </div>
      <div class="find-more">
        <button href="#section1" @click="scrollToSection">
          Dowiedz się więcej
          <img alt="Find more" src="@/assets/bottom.png" />
        </button>
      </div>
    </header>
    <main>
      <section id="section1">
        <div class="wave-box">
          <div style="overflow: hidden">
            <svg
              preserveAspectRatio="none"
              viewBox="0 0 1200 120"
              xmlns="http://www.w3.org/2000/svg"
              style="fill: #ffffff; width: 100%; height: 125px"
            >
              <path
                d="M0 0v46.29c47.79 22.2 103.59 32.17 158 28 70.36-5.37 136.33-33.31 206.8-37.5 73.84-4.36 147.54 16.88 218.2 35.26 69.27 18 138.3 24.88 209.4 13.08 36.15-6 69.85-17.84 104.45-29.34C989.49 25 1113-14.29 1200 52.47V0z"
                opacity=".25"
              />
              <path
                d="M0 0v15.81c13 21.11 27.64 41.05 47.69 56.24C99.41 111.27 165 111 224.58 91.58c31.15-10.15 60.09-26.07 89.67-39.8 40.92-19 84.73-46 130.83-49.67 36.26-2.85 70.9 9.42 98.6 31.56 31.77 25.39 62.32 62 103.63 73 40.44 10.79 81.35-6.69 119.13-24.28s75.16-39 116.92-43.05c59.73-5.85 113.28 22.88 168.9 38.84 30.2 8.66 59 6.17 87.09-7.5 22.43-10.89 48-26.93 60.65-49.24V0z"
                opacity=".5"
              />
              <path
                d="M0 0v5.63C149.93 59 314.09 71.32 475.83 42.57c43-7.64 84.23-20.12 127.61-26.46 59-8.63 112.48 12.24 165.56 35.4C827.93 77.22 886 95.24 951.2 90c86.53-7 172.46-45.71 248.8-84.81V0z"
              />
            </svg>
          </div>
        </div>
        <div class="sec1-box1">
          <div class="box">
            <h1>Rezerwuj online</h1>
            <h2>
              Chcesz zarezerwować miejsce do treningu? Szukasz miejsca, w którym
              spokojnie spędzisz popołudnie ze swoim kompanem?<br /><br />
              Sport+ jest darmową aplikacją, dzięki której z łatwością
              znajdziesz wolny termin i wygodnie zarezerwujesz obiekt
              sportowy.<br /><br />
              Bez dzwonienia, bez umów, bez problemów!
            </h2>
          </div>
          <div class="box">
            <h1>Współpraca z trenerem</h1>
            <h2>
              Jesteś na treningu pierwszy raz?<br /><br />
              Chcesz zacząć swoją przygodę z daną dyscypliną sportu, a może
              zwyczajnie chcesz się podszkolić?<br /><br />
              Świetnie się składa, ponieważ w wybranych obiektach sportowych,
              oprócz rezerwacji miejsca, możesz zarezerwować też trening pod
              okiem wykwalifikowanego trenera.
            </h2>
          </div>
          <div class="box">
            <h1>System punktów i poleceń</h1>
            <h2>
              W Sport+ możesz zbierać wymienne punkty za każdą zrealizowaną
              rezerwację dowolnego obiektu w kraju.<br /><br />
              Punkty możesz zebrać też poprzez polecenie aplikacji nowemu
              użytkownikowi, który założy konto i zrealizuje rezerwację.<br /><br />
              Swoje konto możesz doładować również poprzez zaproszenie znanego
              Ci obiektu do programu Sport+.
            </h2>
          </div>
        </div>
      </section>
      <div class="between-sections"></div>
    </main>
    <footer>
      <div class="footer-box">
        <a>Regulamin</a>
      </div>
      <div class="footer-box-middle">
        <img alt="logo" src="/img/logo.b5767bb6.png" />
        <a>SPORT+</a>
      </div>
      <div class="footer-box">
        <a>FAQ</a>
      </div>
    </footer>
  </body>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    scrollToSection() {
      const section1 = document.querySelector("#section1");
      if (section1) {
        section1.scrollIntoView({ behavior: "smooth" });
      }
    },
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: "smooth" });
    },
  },
};
</script>

<style lang="scss">
#app {
  height: 100%;
  width: 100%;
  margin: 0;
  padding: 0;
}
body {
  margin: 0;
  padding: 0;
  width: 100%;
  height: auto;
  font-size: 16px;
  display: flex;
  align-items: flex-start;
  justify-content: center;
  flex-direction: column;
}
header {
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  flex-direction: column;
}

// navigation
.nav-pc {
  position: fixed;
  top: 0;
  z-index: 2;
  height: 10vh;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: center;
  background-color: #484848;
  border-bottom: 2px solid white;
  outline: 2px solid #484848;
  box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.5);
}
.ul-left,
.ul-right {
  height: 100%;
  width: 45%;
  margin: 0;
  padding: 0;
  list-style-type: none;
}
.ul-left li {
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
.ul-right li {
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
.ul-right img {
  margin-right: 4rem;
  height: 3rem;
  transition: 0.5s;
  border-radius: 50%;
}
.ul-left img {
  margin-left: 4rem;
  height: 3rem;
  transition: 0.5s;
  border-radius: 50%;
}
.ul-right img:hover,
.ul-left img:hover {
  background-color: #eaeaea3c;
}
.logo-nav {
  height: 100%;
  min-width: 235px;
  margin: 0;
  padding: 0;
  border-top-left-radius: 4rem;
  border-top-right-radius: 4rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
.logo-nav button {
  background-color: #22a3da00;
  border: 0;
  cursor: pointer;
}
.logo-nav img {
  height: 5rem;
}

//header-box
.header-box {
  height: 70vh;
  width: 90%;
  background: #22a3da;
  background: radial-gradient(circle, #22a3da 0%, rgba(148, 187, 233, 1) 100%);
  border-radius: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  margin-top: 10%;
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.5);
  border: 1px solid #a3a3a3;
}
.header-main-box {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: center;
}
.header-main-box-left,
.header-main-box-right {
  height: 100%;
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.header-main-box-left {
  background-color: #ffffff16;
  border-radius: 65% 35% 42% 58% / 35% 62% 38% 65%;
  margin-left: 3%;
  height: 95%;
}
.header-main-box-right {
  padding-right: 3%;
  padding-top: 3%;
  justify-content: flex-start;
}
.header-box a {
  font-size: 5rem;
  color: #ffffff;
  padding-left: 2rem;
  cursor: default;
  text-align: center;
  margin: 0;
  padding: 0;
  font-family: "Bebas Neue", sans-serif;
  padding-top: 1%;
}
.header-main-box-right h2 {
  font-size: 1.7rem;
  font-family: "Signika Negative", sans-serif;
  color: #ffffff;
  cursor: default;
  text-align: center;
  margin: 0;
  padding: 0;
}

// find-more
.find-more {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.find-more button {
  font-size: 1.5rem;
  font-family: "Signika Negative", sans-serif;
  font-weight: 700;
  animation: bounce 1.5s infinite;
  cursor: pointer;
  border: 0;
  background-color: #22a3da00;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 5%;
}
.find-more button img {
  height: 30%;
  cursor: pointer;
  animation: bounce 1.5s infinite;
}
@keyframes bounce {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}

// main
main {
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

// section1
#section1 {
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  flex-direction: column;
  background-color: #e4e4e4;
}
.wave-box {
  width: 100%;
  overflow: hidden;
}
.sec1-box1 {
  height: 45%;
  width: 90%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: row;
}
.box {
  height: 80%;
  width: 25%;
  border-radius: 3%;
  border: 1px solid rgb(141, 141, 141);
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.5);
  background: #ffffff;
  background: -webkit-radial-gradient(circle, #ffffff 0%, #eeeeee 100%);
  background: radial-gradient(circle, #ffffff 0%, #eeeeee 100%);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
}
.box h1 {
  font-family: "Bebas Neue", sans-serif;
  font-size: 1.5rem;
  height: 10%;
  cursor: default;
}
.box h2 {
  font-size: 1rem;
  text-align: center;
  font-family: "Signika Negative", sans-serif;
  padding-left: 1%;
  padding-right: 1%;
  height: 90%;
  margin-top: 10%;
  cursor: default;
}

// between-sections
.between-sections {
  height: 25vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
  padding: 0;
  background: url("@/assets/between-sections.jpg");
  background-size: cover; /* Dopasuj obraz do rozmiaru kontenera, zachowując proporcje */
  background-position: center; /* Wyśrodkuj obraz w kontenerze */
  background-repeat: no-repeat;
}
.between-sections img {
  height: 100%;
}

// pod iphone
.find-more-iphone {
  display: none;
}

// footer
footer {
  height: 20vh;
  width: 100%;
  background-color: #484848;
  box-shadow: 0px -15px 15px rgba(0, 0, 0, 0.5);
  z-index: 2;
  border-top: 2px solid white;
  outline: 2px solid #484848;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-around;
}
.footer-box {
  height: 100%;
  width: 33.3%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.footer-box a {
  color: #ffffff;
  font-family: "Signika Negative", sans-serif;
}
.footer-box-middle {
  height: 100%;
  width: 33.3%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.footer-box-middle img {
  height: 50%;
}
.footer-box-middle a {
  color: #ffffff;
  font-family: "Lilita One", cursive;
  font-size: 1.5rem;
}
@media (max-width: 768px) {
  .nav-pc {
    position: fixed;
    top: 0;
    z-index: 3;
    height: 10vh;
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    background-color: #484848;
    border-bottom: 2px solid white;
    outline: 2px solid #484848;
    box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.5);
  }
  .ul-left img {
    height: 2.5rem;
    margin-left: 2rem;
  }
  .ul-right img {
    height: 2.5rem;
    margin-right: 2rem;
  }
  .logo-nav img {
    height: 4.8rem;
  }
  .header-box {
    height: 75%;
    width: 90%;
    background: #22a3da;
    background: radial-gradient(
      circle,
      #22a3da 0%,
      rgba(148, 187, 233, 1) 100%
    );
    border-radius: 2rem;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    margin-top: 25%;
    box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.5);
    border: 1px solid #a3a3a3;
  }
  .header-box a {
    font-size: 2rem;
    color: #ffffff;
    padding-left: 2rem;
    cursor: default;
    text-align: center;
    margin: 0;
    padding: 0;
    font-family: "Bebas Neue", sans-serif;
    padding-top: 5%;
  }
  .header-main-box {
    height: 70%;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
  }
  .header-main-box-left,
  .header-main-box-right {
    height: 50%;

    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }
  .header-main-box-left {
    background-color: #ffffff16;
    border-radius: 65% 35% 42% 58% / 35% 62% 38% 65%;
    margin-left: 0;
  }
  .header-main-box-left img {
    height: 100%;
  }
  .header-main-box-right {
    padding: 0;
    height: auto;
    justify-content: flex-start;
  }

  .header-main-box-right h2 {
    font-size: 1rem;
    font-family: "Signika Negative", sans-serif;
    color: #ffffff;
    cursor: default;
    text-align: center;
    margin: 0;
    padding: 0;
    padding-right: 3%;
    padding-left: 3%;
  }
  .find-more {
    display: none;
  }
  .find-more-iphone {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
  }
  .find-more-iphone {
    height: 40%;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .find-more-iphone button {
    font-size: 1rem;
    font-family: "Signika Negative", sans-serif;
    font-weight: 700;
    animation: bounce 1.5s infinite;
    cursor: pointer;
    border: 0;
    background-color: #22a3da00;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 5%;
    color: #000000;
  }
  .find-more-iphone button img {
    height: 20%;
    cursor: pointer;
    animation: bounce 1.5s infinite;
  }
  #section1 {
    height: 100%;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    flex-direction: column;
    background-color: #e4e4e4;
    padding-bottom: 5rem;
    box-shadow: 0px 10px 15px rgba(0, 0, 0, 0.249);
    z-index: 2;
  }
  .sec1-box1 {
    height: 100%;
    width: 90%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-direction: column;
  }
  .box {
    height: 20rem;
    width: 90%;
    border-radius: 3%;
    border: 1px solid rgb(141, 141, 141);
    box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.5);
    background: #ffffff;
    background: -webkit-radial-gradient(circle, #ffffff 0%, #eeeeee 100%);
    background: radial-gradient(circle, #ffffff 0%, #eeeeee 100%);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    margin-top: 5%;
  }
  .box h2 {
    margin-top: 0;
  }
}
</style>
