<script>
import AppHeader from "./components/AppHeader.vue"

export default {
  components: {AppHeader},
  data() {
    return {
      contributors: [
        {name: "Margaret Glasscoe", organization: "(UAH)", avatarUrl: null},
        {name: "Doug Bausch", organization: "Niyam IT/PDC", avatarUrl: null},
        {name: "Bandana Kar", organization: "Oak Ridge National Laboratory", avatarUrl: null},
        {name: "Prativa Sharma", organization: "University of Missouri-Kansas City", avatarUrl: null},

        {name: "Jun Wang", organization: "Indiana University", avatarUrl: null},
        {name: "Guy Schumann", organization: "ImageCat Inc.", avatarUrl: null},
        {name: "Greg Hempe", organization: "PDC/University of Hawaii", avatarUrl: null},
        {name: "Chris Chiesa", organization: "PDC", avatarUrl: null},

        {name: "Kristy Tiampo", organization: "University of Colorado, Boulder", avatarUrl: null},
        {name: "ZhiQiang Chen", organization: "University of Missouri-Kansas City", avatarUrl: null},
        {name: "Charlie Huyck", organization: "ImageCat Inc.", avatarUrl: null},
        {name: "Ron Eguchi", organization: "ImageCat Inc.", avatarUrl: null}
      ]
    };
  }
}

</script>

<template>
  <div id="app">
    <AppHeader/>

    <section class="section-1">
      <div>
        <h2 class="row-margin">
          Global Flood Map is a <br/>
          ‘GIFFT’ to the World 
        </h2>
        <p class="row-margin border-primary" style="border-left: 3px solid; padding-left: 10px;">
          Funded by the NASA Disasters Program under its Global Initiative for<br/>
          Flood Forecasting and Alerting (GIFFT), Global Flood Map is the first<br/>
          automated source for modeled global flood forecast and inundation<br/>
          information in the world.
        </p>
      </div>
    </section>
    <section class="section-2">
      <div>
        <h2 class="row-margin h2-sub"> INTRODUCTION </h2>
        <h2 class="row-margin"> What is Global Flood Map? </h2>
        <p class="row-margin">
          <b>NASA’s Disasters Program</b> and the <b>University of Hawaii’s Pacific Disaster Center (PDC)</b> have
          partnered to create the <b>first automated source for modeled global flood forecast</b> and inundation
          information in the world.
        </p>
        <div style="background: rgba(41, 64, 211, 0.05);padding-top: 30px;padding-bottom: 30px;">
          <h3 class="row-margin">
            <b-icon icon="check-circle"/>
            Using DisasterAWARE to provide flood warnings.
          </h3>
          <p class="row-margin">
            Based on NASA’s advanced model-of-models approach, the new global flood information will reach tens of
            thousands
            of disaster management decision makers and humanitarian assistance practitioners <b>through PDC’s
            DisasterAWARE
            platform</b> as flood emergencies unfold. <b>DisasterAWARE® will provide flood early warnings</b> and
            supplemental advanced analytical products to help assess potential impacts. 
          </p>
        </div>
      </div>
    </section>
    <section class="section-3">
      <div>
        <h2 class="row-margin h2-sub"> APPROACH </h2>
        <h2 class="row-margin"> Model-of-models approach </h2>
        <p class="row-margin">
          Funded by the NASA Disasters Program under its Global Initiative for Flood Forecasting and Alerting (GIFFT),
          the
          model-of-models approach combines various flood products from open-source models and Earth Observation data to
          determine flood severity risk at sub-watershed level daily and globally. In the current version of this model
          flood outputs from different sources are being leveraged, including:
           
        </p>
        <div class="row-margin d-flex flex-row">
          <div class="w-50">
            <h3>
              <b-icon icon="star-fill"/>
              Forecasting flood severity
            </h3>
            <p> Global Flood Awareness System (GloFAS) and Global Flood Monitoring System (GFMS) data are being used to
              forecast flood severity</p>
          </div>
          <div class="w-50">
            <h3>
              <b-icon icon="star-fill"/>
              Flood severity in near real-time
            </h3>
            <p>MODIS Flood Products from Dartmouth Flood Observatory (DFO/MODIS) and Visible Infrared Imaging Radiometer
              Suite (VIIRS) data are used to determine flood severity in near real-time based on potential
              inundation</p>
          </div>
        </div>
        <div class="row-margin d-flex flex-row" style="margin-bottom: 20px;">
          <div class="w-50" style="margin-right: 20px;">
            <h3>
              <b-icon icon="star-fill"/>
              Flood severity from changing tropical storms
            </h3>
            <p>The Hurricane Weather Research and Forecasting (HWRF) model allows determining flood severity from
              rapidly
              changing tropical storm events. </p>
          </div>
          <div class="w-50">
            <h3>
              <b-icon icon="star-fill"/>
              Trigger alert messages via DisasterAWARE
            </h3>
            <p> The flood severity is then used to trigger alert messages for high-severity flood events via PDC’s
              DisasterAWARE global platform.</p>
          </div>
        </div>
      </div>
    </section>
    <section class="section-4">
      <div>
        <h2 class="row-margin h2-sub"> BENEFITS </h2>
        <h2 class="row-margin">Impacts of the Global Flood map</h2>
        <div class="row-margin d-flex flex-row">
          <div>
            <div class="benefit-icon">
              <img src="./assets/flooded-house-1.png"/>
            </div>
            <h3>Flood extent, depth resolution</h3>
            <p>
              This new technology will be used to create much-needed products that include flood extent and depth at
              finer resolution using Synthetic Aperture Radar (Sentinel 1) data.
            </p>
          </div>

          <div style="margin-left: 20px; margin-right: 20px;">
            <div class="benefit-icon">
              <img src="./assets/mission-1.png"/>
            </div>
            <h3>Anticipate flood impacts</h3>
            <p>
              It will also help anticipate flood impacts on population and critical infrastructures using optical
              imagery as well as geospatial socioeconomic and infrastructure data.
            </p>
          </div>

          <div>
            <div class="benefit-icon">
              <img src="./assets/decision-1.png"/>
            </div>
            <h3>Informed response decisions</h3>
            <p>
              These products aim to allow officials to make more informed disaster response decisions by quickly
              understanding flood severity and extent and their potential impacts to people and property—specifically in
              other parts of the world where flood information is not readily available.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="section-5">
      <div>
        <h2 class="row-margin h2-sub"> PROJECT SUPPORT </h2>
        <h2 class="row-margin">Our Partners</h2>
        <div class="row-margin d-flex flex-row">
          <div>
            <div class="partner-logo">
              <img class="w-100" src="./assets/image-2.png">
            </div>
            <h3>University of Alaska Fairbanks</h3>
          </div>
          <div>
            <div class="partner-logo">
              <img class="w-100" src="./assets/image-3.png">
            </div>
            <h3>Marshall Space Flight Center</h3>
          </div>
          <div>
            <div class="partner-logo">
              <img class="w-100" src="./assets/image-4.png">
            </div>
            <h3>Goddard Space Flight Center</h3>
          </div>
          <div>
            <div class="partner-logo">
              <img class="w-100" src="./assets/image-5.png">
            </div>
            <h3>National Oceanic and Atmospheric Administration</h3>
          </div>
        </div>
      </div>
    </section>

    <section class="section-6">
      <div>
        <h2 class="row-margin h2-sub"> TEAMS </h2>
        <h2 class="row-margin">Contributions and team</h2>
        <div class="row-margin d-flex flex-row flex-wrap">
          <div v-for="(contributor, contributorIndex) in contributors" :key="contributorIndex"
               style="width: 250px; height: 300px;padding: 10px;" class="text-center">
            <div class="contributor-avatar d-inline-block">
              <img v-if="contributor.avatarUrl" class="w-100" :src="contributor.avatarUrl">
              <img v-else class="w-100" src="./assets/Rectangle-7.png">
            </div>
            <h3 class="text-center">{{ contributor.name }}</h3>
            <p class="text-center">{{ contributor.organization }}</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
section {
  background-repeat: no-repeat;
  background-size: 100% 100%;
}

section > div {
}

section.section-1 {
  background-image: url("./assets/image2.png");
}

section.section-2 {
  background-image: url("./assets/image1.png");
}

section.section-3 {
  background-image: url("./assets/Rectangle-5.png");
}

section.section-1 > div {
  padding-top: 200px;
  padding-bottom: 50px;
}

section.section-2 > div {
  padding-top: 80px;
  padding-bottom: 50px;
}

section.section-3 > div {
  padding-top: 50px;
  padding-bottom: 50px;
}

section.section-4 > div {
  padding-top: 50px;
  padding-bottom: 50px;
}

section.section-5 > div {
  padding-top: 50px;
  padding-bottom: 50px;
}

section.section-6 > div {
  padding-top: 50px;
  padding-bottom: 50px;
}


/*section.section-1 h2 {*/
/*  font-family: 'Oswald';*/
/*  font-style: normal;*/
/*  font-weight: 500;*/
/*  font-size: 70px;*/
/*  line-height: 104px;*/
/*  letter-spacing: 0.03em;*/

/*  color: white;*/
/*}*/

section.section-1 p,
section.section-3 p,
section.section-1 h2,
section.section-3 h2,
section.section-1 h3,
section.section-3 h3 {
  color: white;
}

section.section-1 > div {
  background: #2424247d;
}

section.section-3 > div {
  background: #242424f0;
}

section h2.h2-sub {
  font-family: 'Oswald';
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  line-height: 14px;
  letter-spacing: 0.05em;
  color: #2940D3;
  margin-bottom: 0px;
}

section h2 {
  font-family: 'Oswald';
  font-style: normal;
  font-weight: 500;
  font-size: 45px;
  line-height: 59px;
  letter-spacing: 0.03em;
  color: #232323;
  margin-bottom: 25px;
}

section h3 {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 32px;
  letter-spacing: 0.03em;
  color: #2940D3;
}

section.section-3 h3 {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 19px;
  line-height: 32px;
  letter-spacing: 0.03em;
  color: #FFFFFF;
}

section.section-4 h3 {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 17px;
  line-height: 32px;
  letter-spacing: 0.03em;
  color: #000000;
}

section.section-4 .benefit-icon {
  background-color: #2940d31f;
  width: 80px;
  height: 80px;
  border-radius: 40px;
  padding: 15px;
}

section.section-4 .benefit-icon img {
  width: 100%;
  height: 100%;
}

section.section-5 h3 {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 17px;
  line-height: 32px;
  letter-spacing: 0.03em;
  color: #000000;
  padding-left: 30px;
  padding-right: 30px;
  text-align: center;
}

section.section-5 .partner-logo {
  height: 300px;
  padding: 20px;
  display: flex;
  flex-direction: row;
  align-items: end;
}

section.section-6 h3 {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 17px;
  line-height: 32px;
  letter-spacing: 0.03em;
  color: #000000;
  padding-left: 30px;
  padding-right: 30px;
  text-align: center;
}

section.section-6 .contributor-avatar {
  width: 130px;
  height: 150px;
  overflow: hidden;
}

section.section-6 .contributor-avatar img {
  width: 100%;
}

p {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.03em;
}

.row-margin {
  margin-right: 100px;
  margin-left: 100px;
}
</style>
