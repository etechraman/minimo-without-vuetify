<template>
  <div class="main">
    <div class="content">
      <div class="cardsGridBelowDivider">
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
                    class="v-image__image v-image__image--cover"
                    style='background-position: center center;'
                    :style="{ backgroundImage: 'url(' + item.src + ')' }"
                  ></div>
                  <div
                    class="v-responsive__content"
                    style="width: 948px;"
                  ></div>
                </div>
                <div class="v-card__title">
                  <div class="card-heading">LIFESTYLE</div>
                </div>
                <div class="v-card__text card-text">
                  <div class="card-title ">{{ item.title }}</div>
                  <div class="card-description">{{ item.desc }}</div>
                </div>
              </div>
            </div>
          </div>
      </div>
    </div>
    <div class="loadMore">
      <button class="loadMoreButton">Load more</button>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    loading: false,
    selection: 1,
    cards: [
      {
        src: require("../assets/card5.png"),
        title: "Life tastes better with coffee",
        desc: `Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris`,
        cat: "LIFESTYLE",
      },
      {
        src: require("../assets/card6.png"),
        title: "More than just a music festival",
        desc: `Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris`,
        cat: "LIFESTYLE",
      },
    ],
  }),
};
</script>
<style>
.cardsGridBelowDivider {
  padding-top: 52px;
  padding-left: 82px;
}
.loadMore {
  padding-left: 45.14%;
  padding-right: 48.872%;
}
.loadMoreButton {
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 20px !important;
  color: rgba(98, 98, 98, 255) !important;
  padding: 17px 34px;
  width: 164px;
  border: 1px solid #626262;
}
@media only screen and (min-width: 1200px) {
  .cardGridColumn {
    padding: 0px !important;
  }
  .cardImage {
    width: 420px;
  }
}
@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .cardsGridBelowDivider {
    padding: 40px;
    padding-bottom: 0px;
  }
}
@media only screen and (max-width: 960px) {
  .v-card {
    max-width: 100% !important;
  }
  .cardImage {
    width: 900px !important;
    height: 500px !important;
  }
}
@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .cardsGridBelowDivider {
    padding: 40px;
    padding-bottom: 0px;
  }
}
@media only screen and (min-width: 425px) and (max-width: 768px) {
  .cardsGridBelowDivider {
    padding: 40px;
    padding-bottom: 0px;
  }
  .loadMore {
    padding-left: 38.82%;
    padding-right: 0px;
  }
}
@media only screen and (max-width: 425px) {
  .cardsGridBelowDivider {
    padding: 0px;
  }
  .loadMore {
    padding-left: 122px;
    padding-right: 122px;
  }
  .loadMoreButton {
    padding: 5px 12px;
  }
}
@media only screen and  (max-width: 325px) {
  .loadMore {
    padding-left: 0px;
  }
}
</style>
