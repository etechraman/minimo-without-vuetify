<template>
  <div class="cardsDivider">
    <div class="cardsDividerContent">
      <div class="signup">Sign up for our newsletter!</div>
      <div class="enterEmail">
        <div class="container">
          <div class="row">
            <div class="enterEmailAddress col col-12">
              <div
                class="v-input theme--light v-text-field v-text-field--is-booted"
              >
                <div class="v-input__control">
                  <div class="v-input__slot">
                    <div class="v-text-field__slot">
                      <label
                        for="input-16"
                        class="v-label theme--light"
                        style="left: 0px; right: auto; position: absolute;"
                        >Enter a valid email address</label
                      ><input id="input-16" type="text" />
                    </div>
                    <div class="v-input__append-inner">
                      <div class="v-input__icon v-input__icon--clear">
                        <button
                          disabled="disabled"
                          type="button"
                          aria-label="clear icon"
                          class="v-icon notranslate v-icon--disabled v-icon--link mdi mdi-close theme--light"
                        ></button>
                      </div>
                    </div>
                    <div class="v-input__append-inner">
                      <div class="v-image v-responsive theme--light">
                        <div
                          class="v-responsive__sizer"
                          style="padding-bottom: 53.125%;"
                        ></div>
                        <div
                          class="v-image__image v-image__image--cover"
                          style='background-image: url("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAARCAYAAAC8XK78AAABtElEQVRIS8WWPU/bUBSG3/cqoWQJFR2Keu8lRspcKrVLgYGP8H/ozoTKH2JtFJaUCaGyZGtqyQ5iaQVLHSL7HnTTKAoUSALU9WrLz+Nzz3uOubiodwD5IMK6c6h3Op0YOV70LGv1PoCMRCICC+A3IM1icfaw3W5f/kufvsBAYg+Q4yg6OzDGlJRyqyLcBDAH4KcIG+Vy+ajVavWeU2gocFtiFGKMmVdKNkWwCmAGkB/O0R/XKQB5itANgYckRiFBsBCkaaFG4p0XEMFpoZDWw/A8nFbmL4FJJUZASmv9VimpAVwCcEXiyDk24jj+NU7oToFHSAw51Wr1Rbfb/UiK759XAC5IOVRqphmGYfe20L0CT5G4eVzByyzrrQNcA1AiGfnIR1F0AsA9KOBfZIyuK8XmuFJOel9EVgBsA/gOyG4uFUjTdIMUn6ASiVhEfRlbAWv1cC5M+nX+Od8DSZKsKIWNQQ9cktKYqgemhKtK5c2yc9gapKBH4uujUzAJvFJ5vZRlxa3BHIAIvj3LHLgPnsskHIUHQTDrXG8tt11grf7cz+SfbWgAJLltQ2v1J1Le/6//gWuLzA3NP1qxugAAAABJRU5ErkJggg=="); background-position: center center;'
                        ></div>
                        <div
                          class="v-responsive__content"
                          style="width: 32px;"
                        ></div>
                      </div>
                    </div>
                  </div>
                  <div class="v-text-field__details">
                    <div class="v-messages theme--light">
                      <div class="v-messages__wrapper"></div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>
<style>
.cardsDivider {
  width: 100%;
  background-color: #cccccc;
}
.cardsDividerContent {
  max-width: 1200px;
  padding: 4.08% 22.7%;
  margin: 0px auto;
  display: flex;
  flex-direction: column;
  width: max-content;
}
.signup {
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 33px;
  color: rgba(51, 51, 51, 255);
  text-align: center;
}
.enterEmail {
  max-width: 425px;
  margin-top: 83px;
}

.container {
  width: 100%;
  padding: 12px;
  margin-right: auto;
  margin-left: auto;
}
.row {
  display: flex;
  flex-wrap: wrap;
  flex: 1 1 auto;
  /* margin: -12px; */
  margin: 0px !important;
}

.enterEmailAddress {
  padding: 0px !important;
  font-family: PlayfairDisplay-Regular, AdobeInvisFont, MyriadPro-Regular;
  font-size: 14pt;
  color: rgba(98, 98, 98, 255);
  text-align: left;
  margin-right: 32.7%;
}
.col-12 {
  flex: 0 0 100%;
  max-width: 100%;
}
.col {
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
.theme--light.v-input {
  color: rgba(0, 0, 0, 0.87);
}
.v-input {
  align-items: flex-start;
  display: flex;
  flex: 1 1 auto;
  font-size: 16px;
  letter-spacing: normal;
  max-width: 100%;
  text-align: left;
}
.v-text-field {
  padding-top: 12px;
  margin-top: 4px;
}
.v-text-field fieldset,
.v-text-field .v-input__control {
  color: inherit;
}
.v-text-field fieldset,
.v-text-field .v-input__control,
.v-text-field .v-input__slot {
  border-radius: inherit;
}
.v-input__control {
  display: flex;
  flex-direction: column;
  height: auto;
  flex-grow: 1;
  flex-wrap: wrap;
  min-width: 0;
  width: 100%;
}
.v-text-field > .v-input__control > .v-input__slot {
  cursor: text;
}
.v-text-field fieldset,
.v-text-field .v-input__control,
.v-text-field .v-input__slot {
  border-radius: inherit;
}
.v-input__slot {
  align-items: center;
  color: inherit;
  display: flex;
  margin-bottom: 8px;
  min-height: inherit;
  position: relative;
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
  width: 100%;
}
.theme--light.v-text-field > .v-input__control > .v-input__slot:before {
  border-color: rgba(0, 0, 0, 0.42);
}
.v-text-field > .v-input__control > .v-input__slot:before {
  border-color: inherit;
  border-style: solid;
  border-width: thin 0 0 0;
}
.v-text-field > .v-input__control > .v-input__slot:before,
.v-text-field > .v-input__control > .v-input__slot:after {
  bottom: -1px;
  content: "";
  left: 0;
  position: absolute;
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
  width: 100%;
}

.v-text-field > .v-input__control > .v-input__slot > .v-text-field__slot {
  display: flex;
  flex: 1 1 auto;
  position: relative;
}
.theme--light.v-label {
  color: rgba(0, 0, 0, 0.6);
}
.v-input .v-label {
  height: 20px;
  line-height: 20px;
  letter-spacing: normal;
}
.v-text-field .v-label {
  max-width: 90%;
  overflow: hidden;
  text-overflow: ellipsis;
  top: 6px;
  white-space: nowrap;
  pointer-events: none;
}
.v-label {
  font-size: 16px;
  line-height: 1;
  min-height: 8px;
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
}
.theme--light.v-input input,
.theme--light.v-input textarea {
  color: rgba(0, 0, 0, 0.87);
}
.v-input input {
  max-height: 32px;
}
.v-text-field input {
  flex: 1 1 auto;
  line-height: 20px;
  padding: 8px 0 8px;
  max-width: 100%;
  min-width: 0px;
  width: 100%;
}
button,
input,
select,
textarea {
  background-color: transparent;
  border-style: none;
}
button,
input,
optgroup,
select,
textarea {
  font: inherit;
}
input {
  border-radius: 0;
}
button,
input,
select,
textarea {
  font: inherit;
  margin: 0;
}
.v-text-field .v-input__prepend-inner,
.v-text-field .v-input__append-inner {
  align-self: flex-start;
  display: inline-flex;
  margin-top: 4px;
  line-height: 1;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.v-input__icon--clear {
  border-radius: 50%;
}
.v-input__icon {
  align-items: center;
  display: inline-flex;
  height: 24px;
  flex: 1 0 auto;
  justify-content: center;
  min-width: 24px;
  width: 24px;
}
.theme--light.v-icon.v-icon.v-icon--disabled {
  color: rgba(0, 0, 0, 0.38) !important;
}
.v-icon.v-icon.v-icon--link {
  cursor: pointer;
  outline: none;
}
.v-icon.v-icon {
  align-items: center;
  display: inline-flex;
  font-feature-settings: "liga";
  font-size: 24px;
  justify-content: center;
  letter-spacing: normal;
  line-height: 1;
  position: relative;
  text-indent: 0;
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), visibility 0s;
  vertical-align: middle;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.theme--light.v-icon {
  color: rgba(0, 0, 0, 0.54);
}
.v-input__icon--clear .v-icon--disabled {
  visibility: hidden;
}
button,
html [type="button"],
[type="reset"],
[type="submit"] {
  -webkit-appearance: button;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
.v-icon--disabled {
  pointer-events: none;
}
button,
[type="button"],
[type="reset"],
[type="submit"],
[role="button"] {
  cursor: pointer;
  color: inherit;
}
[disabled] {
  cursor: default;
}
button,
input,
select,
textarea {
  background-color: transparent;
  border-style: none;
}
button,
select {
  text-transform: none;
}
button {
  overflow: visible;
}
button,
input,
optgroup,
select,
textarea {
  font: inherit;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button,
select {
  text-transform: none;
}
button {
  overflow: visible;
}
button,
input,
select,
textarea {
  font: inherit;
  margin: 0;
}
.v-icon.v-icon::after {
  background-color: currentColor;
  border-radius: 50%;
  content: "";
  display: inline-block;
  height: 100%;
  left: 0;
  opacity: 0;
  pointer-events: none;
  position: absolute;
  top: 0;
  transform: scale(1.3);
  width: 100%;
  transition: opacity 0.2s cubic-bezier(0.4, 0, 0.6, 1);
}
.v-text-field .v-input__prepend-inner,
.v-text-field .v-input__append-inner {
  align-self: flex-start;
  display: inline-flex;
  margin-top: 4px;
  line-height: 1;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
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

.v-text-field > .v-input__control > .v-input__slot:after {
  background-color: currentColor;
  border-color: currentColor;
  border-style: solid;
  border-width: thin 0 thin 0;
  transform: scaleX(0);
}
.v-text-field > .v-input__control > .v-input__slot:before,
.v-text-field > .v-input__control > .v-input__slot:after {
  bottom: -1px;
  content: "";
  left: 0;
  position: absolute;
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
  width: 100%;
}
.v-text-field__details {
  display: flex;
  flex: 1 0 auto;
  max-width: 100%;
  min-height: 14px;
  overflow: hidden;
}
.theme--light.v-messages {
  color: rgba(0, 0, 0, 0.6);
}
.v-messages {
  flex: 1 1 auto;
  font-size: 12px;
  min-height: 14px;
  min-width: 1px;
  position: relative;
}
@media (min-width: 960px) {
  .container {
    max-width: 900px;
  }
}
@media only screen and (max-width: 1200px) {
  .cardsDividerContent {
    width: 100% !important;
    padding: 4.01% 22.35% !important;
    margin: 0px auto;
    align-items: center;
  }
  .enterEmail v-img {
    width: 50px;
  }
}
@media (min-width: 1264px) {
  .container {
    max-width: 1185px;
  }
}

</style>
