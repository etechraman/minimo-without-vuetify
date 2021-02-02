<template>
  <div class="footer">
    <div class="terms">Terms and conditions</div>
    <div class="privacy">Privacy</div>
    <div class="socialHandle">
      <div class="follow">Follow</div>
      <div class="facebook">
        <img width="" height="14px" src="../assets/facebook.png" alt="" />
      </div>
      <div class="twitter">
        <img width="" height="13px" src="../assets/twitter.png" alt="" />
      </div>
      <div class="instagram">
        <img width="" height="15px" src="../assets/instagram.png" alt="" />
      </div>
    </div>
  </div>
</template>
<style>
.footer {
  width: 100%;
  display: flex;
  margin-top: 1370px;
  height: 97px;
  background-color: #f0f0f0;
}

.terms {
  font-size: 14px;
  line-height: 24px;
  color: #000000;
  font-weight: 400;
  font-family: "Playfair Display";
  padding-top: 40px;
  padding-bottom: 45px;
  width: 136px !important;
  margin-left: 8.162%;
}
.privacy {
  font-size: 14px;
  line-height: 24px;
  color: #000000;
  font-weight: 400;
  font-family: "Playfair Display";
  padding-top: 40px;
  padding-bottom: 45px;
  width: 46px;
  margin-right: 0.925%;
}
.socialHandle {
  display: flex;
  margin-left: auto;
  margin-right: 3.863%;
}
.follow {
  font-size: 14px;
  line-height: 24px;
  color: #000000;
  font-weight: 400;
  font-family: "Playfair Display";
  padding-top: 40px;
  padding-bottom: 45px;
  width: 42px;
  margin-left: auto;
  margin-right: 15.12%;
}
.facebook {
  font-size: 14px;
  line-height: 24px;
  color: #000000;
  font-weight: 400;
  font-family: "Playfair Display";
  padding-top: 40px;
  padding-bottom: 44px;
  margin-left: 17.8%;
  padding-bottom: 43px;
}
.twitter {
  font-size: 14px;
  line-height: 24px;
  color: #000000;
  font-weight: 400;
  font-family: "Playfair Display";
  padding-top: 40px;
  padding-bottom: 44px;
  margin-left: 17%;
}
.instagram {
  padding-top: 40px;
  padding-bottom: 42px;
  margin-left: 21.8%;
}

@media only screen and (min-width: 768px) and (max-width: 1440px) {
  .socialHandle {
    margin-right: 7.863%;
  }
}

@media only screen and (max-width: 768px) {
  .footer {
    height: auto;
    display: flex;
    flex-direction: column;
  }
  .terms {
    width: auto !important;
    margin-left: 2%;
    padding-top: 8px;
    padding-bottom: 8px;
  }
  .privacy {
    margin-left: 2%;
    padding-top: 8px;
    padding-bottom: 8px;
  }
  .socialHandle {
    margin-left: 0px;
    padding-top: 8px;
    padding-bottom: 8px;
    flex-direction: column;
  }
  .follow {
    margin-left: 2%;
    padding-top: 8px;
    padding-bottom: 8px;
  }
  .facebook {
    margin-left: 2%;
    padding-top: 8px;
    padding-bottom: 8px;
  }
  .twitter {
    margin-left: 2%;
    padding-top: 8px;
    padding-bottom: 8px;
  }
  .instagram {
    margin-left: 2%;
    padding-top: 8px;
    padding-bottom: 8px;
  }
}
</style>
