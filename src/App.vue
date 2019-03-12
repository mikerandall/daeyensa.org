<template>
  <b-container fluid id="app">
    <lead></lead>
    <schedule></schedule>
    <ceremonies></ceremonies>
    <contact></contact>
    <foot></foot>
  </b-container>
</template>

<script>
import Lead from './Lead.vue';
import Schedule from './Schedule.vue';
import Ceremonies from './Ceremonies.vue';
import Contact from './Contact.vue';
import Foot from './Foot.vue';

export default {
  name: 'app',
  data () {
    return {
      title: 'Welcome to Dae Yen Sa Temple!'
    }
  },
  components: {
    Lead,
    Schedule,
    Ceremonies,
    Contact,
    Foot
  }
}
</script>

<style lang="scss">
/* cyrillic-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4ARPQ_mu72BiBLE.woff2) format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
/* cyrillic */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4ARGQ_mu72BiBLE.woff2) format('woff2');
  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
/* devanagari */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4ARDQ_mu72BiBLE.woff2) format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF6, U+1CF8-1CF9, U+200C-200D, U+20A8, U+20B9, U+25CC, U+A830-A839, U+A8E0-A8FB;
}
/* greek-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4AROQ_mu72BiBLE.woff2) format('woff2');
  unicode-range: U+1F00-1FFF;
}
/* greek */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4ARBQ_mu72BiBLE.woff2) format('woff2');
  unicode-range: U+0370-03FF;
}
/* vietnamese */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4ARNQ_mu72BiBLE.woff2) format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+1EA0-1EF9, U+20AB;
}
/* latin-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4ARMQ_mu72BiBLE.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: normal;
  src: local('Noto Sans Italic'), local('NotoSans-Italic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0OIpQlx3QUlC5A4PNr4ARCQ_mu72Bi.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
/* cyrillic-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyOzW1IPriezag.woff2) format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
/* cyrillic */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyHzW1IPriezag.woff2) format('woff2');
  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
/* devanagari */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyCzW1IPriezag.woff2) format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF6, U+1CF8-1CF9, U+200C-200D, U+20A8, U+20B9, U+25CC, U+A830-A839, U+A8E0-A8FB;
}
/* greek-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyPzW1IPriezag.woff2) format('woff2');
  unicode-range: U+1F00-1FFF;
}
/* greek */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyAzW1IPriezag.woff2) format('woff2');
  unicode-range: U+0370-03FF;
}
/* vietnamese */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyMzW1IPriezag.woff2) format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+1EA0-1EF9, U+20AB;
}
/* latin-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyNzW1IPriezag.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Noto Sans';
  font-style: italic;
  font-weight: bold;
  src: local('Noto Sans Bold Italic'), local('NotoSans-BoldItalic'), url(https://fonts.gstatic.com/s/notosans/v8/o-0TIpQlx3QUlC5A4PNr4Az5ZuyDzW1IPrie.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
/* cyrillic-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr6DRASf6M7VBj.woff2) format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
/* cyrillic */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr4TRASf6M7VBj.woff2) format('woff2');
  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
/* devanagari */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr5DRASf6M7VBj.woff2) format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF6, U+1CF8-1CF9, U+200C-200D, U+20A8, U+20B9, U+25CC, U+A830-A839, U+A8E0-A8FB;
}
/* greek-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr6TRASf6M7VBj.woff2) format('woff2');
  unicode-range: U+1F00-1FFF;
}
/* greek */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr5jRASf6M7VBj.woff2) format('woff2');
  unicode-range: U+0370-03FF;
}
/* vietnamese */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr6jRASf6M7VBj.woff2) format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+1EA0-1EF9, U+20AB;
}
/* latin-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr6zRASf6M7VBj.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: normal;
  src: local('Noto Sans'), local('NotoSans'), url(https://fonts.gstatic.com/s/notosans/v8/o-0IIpQlx3QUlC5A4PNr5TRASf6M7Q.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
/* cyrillic-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVadyBx2pqPIif.woff2) format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
/* cyrillic */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVYNyBx2pqPIif.woff2) format('woff2');
  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
/* devanagari */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVZdyBx2pqPIif.woff2) format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF6, U+1CF8-1CF9, U+200C-200D, U+20A8, U+20B9, U+25CC, U+A830-A839, U+A8E0-A8FB;
}
/* greek-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVaNyBx2pqPIif.woff2) format('woff2');
  unicode-range: U+1F00-1FFF;
}
/* greek */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVZ9yBx2pqPIif.woff2) format('woff2');
  unicode-range: U+0370-03FF;
}
/* vietnamese */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVa9yBx2pqPIif.woff2) format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+1EA0-1EF9, U+20AB;
}
/* latin-ext */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVatyBx2pqPIif.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: bold;
  src: local('Noto Sans Bold'), local('NotoSans-Bold'), url(https://fonts.gstatic.com/s/notosans/v8/o-0NIpQlx3QUlC5A4PNjXhFVZNyBx2pqPA.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}

body {
  font-family: 'Noto Sans', Helvetica, Arial, sans-serif;
  font-size: 19px;
  letter-spacing: -0.98px;
  line-height: 28px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#app {
  color: #2c3e50;
  text-align: left;
}

.container-fluid {
  padding-left: 0;
  padding-right: 0;
}


h1, h2 {
  color: #BF1932;
  font-family: 'Noto Sans';
  font-weight: bold;
  margin: 20px 0 40px;
}

h2 {
  font-size: 30px;
  letter-spacing: -2.32px;
}

h3 {
  font-family: 'Noto Sans';
  font-weight: bold;
  font-style: italic;
  font-size: 30px;
  color: #000000;
  margin: 20px 0 40px;
}

h4 {
  font-family: 'Noto Sans';
  font-weight: bold;
  font-size: 20px;
  color: #000000;
  margin: 20px 0 40px;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

p, address {
  font-size: 15px;
}

@media (min-width: 576px) {
  h2 {
    font-size: 38px;
  }

  h3 {
    font-size: 38px;
  }

  h4 {
    font-size: 22px;
  }

  p {
    font-size: 19px;
  }
}

@media (min-width: 768px) {
  h2 {
    font-size: 45px;
    letter-spacing: -2.32px;
  }

  h3 {
    font-size: 30px;
    margin: 20px 0 40px;
  }

  h4 {
    font-size: 30px;
    margin: 20px 0 40px;
  }

}
</style>
