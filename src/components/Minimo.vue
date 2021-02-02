<template>
  <div>
    <div class="navBarButton">
      <header class="w3-container headBar">
        <span class="w3-opennav w3-xlarge">
          <div
            class="menuContainer"
            v-click-outside="onClickOutside"
            @click="handleMenuClick()"
          >
            <div class="bar1"></div>
            <div class="bar2"></div>
            <div class="bar3"></div>
          </div>
        </span>
      </header>
      <nav
        ref="sidenav"
        class="w3-sidenav w3-white w3-card-2 sideNav"
        style="display:none"
      >
        <a>
          <img
            width=""
            height=""
            aspect-ratio="5.173"
            class="minimologo"
            src="../assets/minimologo.png"
            alt="LOGO"
          />
        </a>
        <a class="lifestyle">LIFESTYLE</a>
        <a class="photodiary">PHOTODIARY</a>
        <a class="music">MUSIC</a>
        <a class="travel">TRAVEL</a>
      </nav>
    </div>
    <div class="main">
      <nav v-show="true">
        <div class="d-flex topbar">
          <img
            width=""
            height=""
            aspect-ratio="5.173"
            class="minimologo"
            src="../assets/minimologo.png"
            alt="LOGO"
          />
          <div class="d-flex nav-right">
            <div class="lifestyle">LIFESTYLE</div>
            <div class="photodiary">PHOTODIARY</div>
            <div class="music">MUSIC</div>
            <div class="travel">TRAVEL</div>
          </div>
        </div>
      </nav>
      <div class="content">
        <div class="firstpost">
          <img
            width="99.8125%"
            aspect-ratio="1.574"
            height=""
            src="../assets/firstpost.png"
            alt=""
          />
        </div>
        <div class="contentBelowFirstPost">PHOTODIARY</div>
        <div class="contentFirstPostTitle">The perfect weekend getaway</div>
        <div class="contentFirstPostDescription">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. Duis aute irure dolor in
            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
            pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt mollit anim id est laborum. Sed ut
            perspiciatis unde omnis iste natus error sit voluptatem accusantium
            doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
            inventore veritatis et quasi architecto beatae vitae dicta sunt
            explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur
            aut odit aut fugit, sed quia consequuntur magni dolores eos qui
            ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui
            dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed
            quia non numquam eius modi tempora incidunt ut labore et dolore
            magnam aliquam quaerat voluptatem.
          </p>
        </div>
        <div class="contentFirstPostComment">LEAVE A COMMENT</div>

        <div class="cardsGrid">
          <div class="row">
            <div
              class="col col-sm-12 col-xs-12 col-md-6 col-lg-6 cardGridColumn d-flex justify-center"
              v-for="(item, index) in cards"
              :key="index"
            >
              <div class="v-card v-sheet theme--light">
                <div
                  class="v-image v-responsive cardImage theme--light"
                  fluid=""
                  style="height: 280px;"
                >
                  <div
                    class="v-responsive__sizer"
                    style="padding-bottom: 66.6667%;"
                  ></div>
                  <div
                    ref="cardImagePng"
                    class="v-image__image v-image__image--cover"
                    style='background-position: center center;'
                    :style="{ backgroundImage: 'url(' + item.src + ')' }"
                    
                  ></div>

                  <div
                    class="v-responsive__content"
                    style="width: 948px;"
                  ></div>
                </div>
                <!-- <v-img
                  v-show="true"
                  class="cardImage"
                  ref="cardImage"
                  fluid
                  height="280"
                  :src="item.src"
                ></v-img> -->

                <div class="v-card__title">
                  <div class="card-heading">LIFESTYLE</div>
                </div>
                <!-- 
                <v-card-title>
                  <div class="card-heading">{{ item.cat }}</div>
                </v-card-title> -->

                <div class="v-card__text card-text">
                  <div class="card-title ">{{ item.title }}</div>
                  <div class="card-description">{{ item.desc }}</div>
                </div>

                <!-- <v-card-text class="card-text">
                  <div class="card-title ">
                    {{ item.title }}
                  </div>

                  <div class="card-description">
                    {{ item.desc }}
                  </div>
                </v-card-text> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import vClickOutside from "v-click-outside";
export default {
  data() {
    return {
      loading: false,
      directives: {
        clickOutside: vClickOutside.directive,
      },
      cards: [
        {
          src: require("../assets/card1.png"),
          title: "Life tastes better with coffee",
          desc: `Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris`,
          cat: "LIFESTYLE",
        },
        {
          src: require("../assets/card2.png"),
          title: "More than just a music festival",
          desc: `Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris`,
          cat: "LIFESTYLE",
        },
        {
          src: require("../assets/card3.png"),
          title: "American dream",
          desc: `Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris`,
          cat: "PHOTODIARY",
        },
        {
          src: require("../assets/card4.png"),
          title: "A day exploring the Alps",
          desc: `Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris`,
          cat: "PHOTODIARY",
        },
      ],
    };
  },
  mounted() {
    // this.$refs.cardImagePng.style.backgroundImage='url(' + imgArray[curIndex % 3] + ')';
  },
  methods: {
    onClickOutside() {
      if (this.$refs.sidenav.style.display === "block") this.closeMenu();
      else return;
    },
    handleMenuClick() {
      if (this.$refs.sidenav.style.display === "none") this.openMenu();
      else {
        this.closeMenu();
      }
    },
    openMenu() {
      document
        .getElementsByClassName("menuContainer")[0]
        .classList.toggle("change");
      this.$refs.sidenav.style.display = "block";
    },
    closeMenu() {
      document
        .getElementsByClassName("menuContainer")[0]
        .classList.toggle("change");
      this.$refs.sidenav.style.display = "none";
    },

    reserve() {
      this.loading = true;

      setTimeout(() => (this.loading = false), 2000);
    },
  },
};
</script>

<style>
@import "../assets/stylesheets/stylesheet.css";
.headBar {
  width: 100%;
  z-index: 9999;
}
.sideNav {
  margin-top: 40px !important;
}

.main {
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding: 68px;
  padding-bottom: 0px;
}
nav {
  height: 26px;
}
.minimo {
  font-family: Inconsolata-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 30pt;
  color: rgba(0, 0, 0, 255);
  text-align: center;
  margin-right: 36.84%;
}

.menuContainer {
  display: inline-block;
  cursor: pointer;
  margin-right: 23px;
}

.bar1,
.bar2,
.bar3 {
  width: 35px;
  height: 5px;
  background-color: #333;
  margin: 6px 0;
  transition: 0.4s;
}

.change .bar1 {
  -webkit-transform: rotate(-45deg) translate(-9px, 6px);
  transform: rotate(-45deg) translate(-9px, 6px);
}

.change .bar2 {
  opacity: 0;
}

.change .bar3 {
  -webkit-transform: rotate(45deg) translate(-8px, -8px);
  transform: rotate(45deg) translate(-8px, -8px);
}

.topbar {
  display: flex;
  width: auto;
}
.topbar .minimologo {
  margin-right: 35.84%;
}

.nav-right {
  display: flex;
  width: auto;
}

.topbar div,
.lifestyle,
.photodiary,
.music,
.travel {
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 14px;
  color: rgba(98, 98, 98, 255);
  text-align: center;
}
.topbar .lifestyle {
  margin-right: 40.5%;
}
.topbar .photodiary {
  margin-right: 39.5%;
}
.topbar .music {
  margin-right: 36.43%;
}
.firstpost {
  margin-bottom: 99px;
}
.contentBelowFirstPost {
  font-family: Ubuntu-Light, AdobeInvisFont, MyriadPro-Regular;
  font-size: 16px;
  color: rgba(180, 173, 158, 255);
  text-align: left;
  padding-left: 7.7%;
}
.contentFirstPostTitle {
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 30pt;
  color: rgba(98, 98, 98, 255);
  text-align: left;
  padding-left: 7.69%;
  margin-top: 2.63%;
  margin-bottom: 3.2%;
}
.contentFirstPostDescription {
  padding-left: 7.528%;
  padding-right: 8.359%;
}
.contentFirstPostDescription p {
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 16px;
  color: rgba(98, 98, 98, 255);
  text-align: left;
  margin-bottom: 52px;
}
.contentFirstPostComment {
  font-family: Ubuntu-Light, AdobeInvisFont, MyriadPro-Regular;
  font-size: 16px;
  color: rgba(180, 173, 158, 255);
  text-align: left;
  padding-left: 7.7%;
}
.cardsGrid {
  padding-left: 82px;
  padding-top: 134px;
}
.row {
  margin: 0px !important;
  display: flex;
  flex-wrap: wrap;
  flex: 1 1 auto;
  margin: -12px;
}
.col {
  display: flex;
  justify-content: center;
  flex-basis: 0;
  flex-grow: 1;
  max-width: 100%;
}
.col-xl,
.col-xl-auto,
.col-xl-12,
.col-xl-11,
.col-xl-10,
.col-xl-9,
.col-xl-8,
.col-xl-7,
.col-xl-6,
.col-xl-5,
.col-xl-4,
.col-xl-3,
.col-xl-2,
.col-xl-1,
.col-lg,
.col-lg-auto,
.col-lg-12,
.col-lg-11,
.col-lg-10,
.col-lg-9,
.col-lg-8,
.col-lg-7,
.col-lg-6,
.col-lg-5,
.col-lg-4,
.col-lg-3,
.col-lg-2,
.col-lg-1,
.col-md,
.col-md-auto,
.col-md-12,
.col-md-11,
.col-md-10,
.col-md-9,
.col-md-8,
.col-md-7,
.col-md-6,
.col-md-5,
.col-md-4,
.col-md-3,
.col-md-2,
.col-md-1,
.col-sm,
.col-sm-auto,
.col-sm-12,
.col-sm-11,
.col-sm-10,
.col-sm-9,
.col-sm-8,
.col-sm-7,
.col-sm-6,
.col-sm-5,
.col-sm-4,
.col-sm-3,
.col-sm-2,
.col-sm-1,
.col,
.col-auto,
.col-12,
.col-11,
.col-10,
.col-9,
.col-8,
.col-7,
.col-6,
.col-5,
.col-4,
.col-3,
.col-2,
.col-1 {
  width: 100%;
  padding: 12px;
}

.cardGridColumn {
  margin-bottom: 130px;
}
.v-sheet.v-card:not(.v-sheet--outlined) {
  box-shadow: 0px 3px 1px -2px rgb(0 0 0 / 20%),
    0px 2px 2px 0px rgb(0 0 0 / 14%), 0px 1px 5px 0px rgb(0 0 0 / 12%);
}
.v-sheet.v-card:not(.v-sheet--outlined) {
  box-shadow: none !important;
}
.v-sheet:not(.v-sheet--outlined) {
  box-shadow: 0px 0px 0px 0px rgb(0 0 0 / 20%), 0px 0px 0px 0px rgb(0 0 0 / 14%),
    0px 0px 0px 0px rgb(0 0 0 / 12%);
}
.theme--light.v-sheet {
  background-color: #ffffff;
  border-color: #ffffff;
  color: rgba(0, 0, 0, 0.87);
}
.v-sheet.v-card {
  border-radius: 4px;
}
.theme--light.v-card {
  background-color: #ffffff;
  color: rgba(0, 0, 0, 0.87);
}
.v-sheet {
  border-radius: 0;
}
.v-card {
  border-width: thin;
  display: block;
  max-width: 100%;
  outline: none;
  text-decoration: none;
  transition-property: box-shadow, opacity;
  overflow-wrap: break-word;
  position: relative;
  white-space: normal;
}

.v-card > *:first-child:not(.v-btn):not(.v-chip),
.v-card > .v-card__progress + *:not(.v-btn):not(.v-chip) {
  border-top-left-radius: inherit;
  border-top-right-radius: inherit;
}
.theme--light.v-image {
  color: rgba(0, 0, 0, 0.87);
}

.v-responsive {
  position: relative;
  overflow: hidden;
  flex: 1 0 auto;
  max-width: 100%;
  display: flex;
}
.v-image {
  z-index: 0;
}

.v-responsive__sizer {
  transition: padding-bottom 0.2s cubic-bezier(0.25, 0.8, 0.5, 1);
  flex: 1 0 0px;
}

.v-image__image--cover {
  background-size: cover;
}
.v-image__image {
  background-repeat: no-repeat;
}
.v-image__image,
.v-image__placeholder {
  z-index: -1;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.v-responsive__content {
  flex: 1 0 0px;
  max-width: 100%;
}

.v-card__title {
  align-items: center;
  display: flex;
  flex-wrap: wrap;
  font-size: 1.25rem;
  font-weight: 500;
  letter-spacing: 0.0125em;
  line-height: 2rem;
  word-break: break-all;
}
.v-card__subtitle,
.v-card__text,
.v-card__title {
  padding: 16px;
}
.v-card__subtitle,
.v-card__text,
.v-card__title {
  padding: 0px 0px !important;
}
.v-card__subtitle,
.v-card__text,
.v-card__title {
  padding: 0px 0px !important;
}
.card-heading {
  font-family: Ubuntu-Light, AdobeInvisFont, MyriadPro-Regular;
  font-size: 14pt;
  color: rgba(180, 173, 158, 255);
  text-align: left;
  margin-top: 12px;
}

.v-card > *:last-child:not(.v-btn):not(.v-chip) {
  border-bottom-left-radius: inherit;
  border-bottom-right-radius: inherit;
}
.theme--light.v-card > .v-card__text,
.theme--light.v-card .v-card__subtitle {
  color: rgba(0, 0, 0, 0.6);
}
.v-card__title + .v-card__subtitle,
.v-card__title + .v-card__text {
  padding-top: 0;
}
.v-card__text {
  width: 100%;
}
.v-card__subtitle,
.v-card__text,
.v-card__title {
  padding: 16px;
}
.v-card__subtitle,
.v-card__text {
  font-size: 0.875rem;
  font-weight: 400;
  line-height: 1.375rem;
  letter-spacing: 0.0071428571em;
}
.card-text {
  padding: 20px 0px;
}

.v-card__subtitle,
.v-card__text,
.v-card__title {
  padding: 0px 0px !important;
}

.card-title {
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 33px;
  line-height: 33px;
  color: rgba(98, 98, 98, 255);
  text-align: left;
  padding: 20px 0px;
  margin-bottom: 18px;
}
.card-description {
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 17px;
  color: rgba(98, 98, 98, 255);
  text-align: left;
}

@media only screen and (min-width: 180px) and (max-width: 425px) {
  nav {
    display: none;
  }
  .main {
    padding: 8px;
    padding-bottom: 0px;
  }
  .contentFirstPostTitle {
    font-size: 24pt;
  }
  .cardsGrid {
    padding: 0px;
  }
}
@media only screen and (min-width: 425px) and (max-width: 768px) {
  nav {
    display: none;
  }
  .main {
    padding: 8px;
    padding-bottom: 0px;
  }
  .contentFirstPostTitle {
    font-size: 24pt;
  }
  .cardsGrid {
    padding: 40px;
    padding-bottom: 0px;
  }
}
@media (min-width: 600px) {
  .col-sm-12 {
    flex: 0 0 100%;
    max-width: 100%;
  }
}
@media only screen and (min-width: 768px) and (max-width: 1024px) {
  nav {
    display: none;
  }
  .main {
    padding: 8px;
    padding-bottom: 0px;
  }
  .contentFirstPostTitle {
    font-size: 30pt;
  }
  .cardsGrid {
    padding: 40px;
    padding-bottom: 0px;
  }
}
@media (min-width: 960px) {
  .col-md-6 {
    flex: 0 0 50%;
    max-width: 50%;
  }
}

@media only screen and (min-width: 1024px) and (max-width: 1200px) {
  nav {
    display: none;
  }
  .main {
    padding: 8px;
    padding-bottom: 0px;
  }
  .cardsGrid {
    padding: 40px;
    padding-bottom: 0px;
  }
}
@media only screen and (min-width: 1200px) {
  .cardImage {
    width: 420px;
  }
  .navBarButton {
    display: none;
  }
}
@media (min-width: 1264px) {
  .col-lg-6 {
    flex: 0 0 50%;
    max-width: 50%;
  }
}
</style>
