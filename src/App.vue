<script>
import AppHeader from "./components/AppHeader.vue"

export default {
  components: {AppHeader},
  data() {
    return {
      contributors: [
        {name: "Margaret Glasscoe", organization: "(UAH)", avatarUrl: "./assets/team-members/Glasscoe_Margaret.jpg"},
        {name: "Doug Bausch", organization: "Niyam IT/PDC", avatarUrl: "./assets/team-members/Bausch_Doug.png"},
        {name: "Bandana Kar", organization: "Oak Ridge National Laboratory", avatarUrl: "./assets/team-members/Kar_Bandana.jpg"},
        {name: "Prativa Sharma", organization: "University of Missouri-Kansas City", avatarUrl: null},

        {name: "Jun Wang", organization: "Indiana University", avatarUrl: "./assets/team-members/Wang_Jun.jpg"},
        {name: "Guy Schumann", organization: "ImageCat Inc.", avatarUrl: "./assets/team-members/Schumann_Guy.jpg"},
        {name: "Greg Hampe", organization: "University of Hawaii/PDC", avatarUrl: "./assets/team-members/Hampe_Greg.jpg"},
        {name: "Chris Chiesa", organization: "University of Hawaii/PDC", avatarUrl: "./assets/team-members/Chiesa_Chris.jpg"},

        {name: "Kristy Tiampo", organization: "University of Colorado, Boulder", avatarUrl: "./assets/team-members/Tiampo_Kristy.jpg"},
        {name: "ZhiQiang Chen", organization: "University of Missouri-Kansas City", avatarUrl: "./assets/team-members/Chen_ZQ.png"},
        {name: "Charlie Huyck", organization: "ImageCat Inc.", avatarUrl: "./assets/team-members/Huyck_Charlie.jpg"},
        {name: "Ron Eguchi", organization: "ImageCat Inc.", avatarUrl: "./assets/team-members/Eguchi_Ron.png"}
      ],
      publications: [
        {
          title: `Margaret Glasscoe, Douglas Bausch, Prativa Sharma, Jun Wang, ZhiQiang Chen, Molan Zhang, Guy Schumann, Marlon Pierce, Clay Woods, Kristy Tiampo, Ronald Eguchi (2021). Integrating Hydrologic Models and Earth Observation Data for Global Flood Forecasting and Alerting In Near Real-Time. IGARSS International Geosciences and Remote Sensing Symposium, Brussels, Belgium.`,
          pdf: "#"
        },
        {
          title: `K. Tiampo, C. Woods, L. Huang, P. Sharma, Z. Chen , B. Kar, D. Bausch, C. Simmons, R. Estrada, M. Willlis, M. Glasscoe (2021) A MACHINE LEARNING APPROACH TO FLOOD DEPTH AND EXTENT DETECTION USING SENTINEL 1A/B SYNTHETIC APERTURE RADAR. IGARSS International Geosciences and Remote Sensing Symposium, Brussels, Belgium.`,
          pdf: "#"
        },
        {
          title: `M.Zhang and Z. Chen (2021) Deep Metric Learning for Damage Detection Using Bitemporal Satellite Images, IGARSS International Geosciences and Remote Sensing Symposium, Brussels, Belgium.`,
          pdf: "#"
        },
        {
          title: `BANDANA KAR, DOUG BAUSCH, JUN WANG, PRATIVA SHARMA, ZHIQIANG CHEN, GUY SCHUMANN, MARLON PIERCE, KRISTY TIAMPO, RON EGUCHI, MARGARET GLASSCOE (2020). "INTEGRATED MODEL OF MODELS FOR GLOBAL FLOOD ALERTING." WIT Transactions on the Built Environment, v. 194, p. 73-83.`,
          pdf: "#"
        },
        {
          title: `P Sharma, J Wang, M Zhang, C Woods, B Kar, D Bausch, Z Chen, K Tiampo, M Glasscoe, G Schumann, M Pierce, R Eguchi (2020). "DisasterAWARE–A GLOBAL ALERTING PLATFORM FOR FLOOD EVENTS." ISPRS Annals of the Photogrammetry, Remote Sensing and Spatial Information Sciences, v 6, p. 107-113.`,
          pdf: "#"
        },
        {
          title: `Chen, Z., Glasscoe, M.T., Eguchi, R., Huyck, C., and Kar, Bandana (2020). Roles of Remote Sensing Technologies in Disaster Resilience. Objective Resilience Primer Manual of Practice (ASCE Objective Resilience Committee, editor: Mohammad Ettouney). In Press.`,
          pdf: "#"
        },
        {
          title: `B. Kar, D. Bausch, J. Wang, P. Sharma, Z. Chen, G. Schumann, M. Pierce, K. Tempo, R. Eguchi, M. Glasscoe (2020). “An Integrated Model of Models for Global Flood Alerting”. 7th International Conference on Flood and Urban Water Management (FRIAR 2020). Valencia, Spain.`,
          pdf: "#"
        },
        {
          title: `Chen, Z., Glasscoe, M.T., Eguchi, R., Huyck, C., and Kar, Bandana (2020). “Roles of Remote Sensing Technologies in Disaster Resilience.” To appear in Objective Resilience Primer Manual of Practice (ASCE Objective Resilience Committee, editor: Mohammad Ettouney).`,
          pdf: "#"
        },
        {
          title: `Prativa Sharma, B. Kar, Z. Chen, D. Bausch, J. Wang, G. Schumann, M. Pierce, K. Tempo, R. Eguchi, M. Glasscoe (2020). “MOM- An Integrated Model of Models for Global Flood Alerting and Impact Assessment”. AAG. Denver, CO.`,
          pdf: "#"
        }
      ],
      presentations: [
        {
          title: `K. Bedka and M. Glasscoe (2021) NASA Disasters Program Overview and Response to Africa Floods, UN-SPIDER / ZFL Regional Virtual Expert Meeting for Southern Africa "Space-based Solutions for Disaster Risk Management and Emergency Response"`,
          pdf: "#"
        },
        {
          title: `Margaret Glasscoe, Douglas Bausch, Prativa Sharma, Jun Wang, ZhiQiang Chen, Molan Zhang, Guy Schumann, Marlon Pierce, Clay Woods, Kristy Tiampo, Ronald Eguchi (2021). Integrating Hydrologic Models and Earth Observation Data for Global Flood Forecasting and Alerting In Near Real-Time. IGARSS International Geosciences and Remote Sensing Symposium, Brussels, Belgium.`,
          pdf: "#"
        },
        {
          title: `K. Tiampo, C. Woods, L. Huang, P. Sharma, Z. Chen , B. Kar, D. Bausch, C. Simmons, R. Estrada, M. Willlis, M. Glasscoe (2021) A MACHINE LEARNING APPROACH TO FLOOD DEPTH AND EXTENT DETECTION USING SENTINEL 1A/B SYNTHETIC APERTURE RADAR. IGARSS International Geosciences and Remote Sensing Symposium, Brussels, Belgium.`,
          pdf: "#"
        },
        {
          title: `M.Zhang and Z. Chen (2021) Deep Metric Learning for Damage Detection Using Bitemporal Satellite Images, IGARSS International Geosciences and Remote Sensing Symposium, Brussels, Belgium.`,
          pdf: "#"
        },
        {
          title: `M.Glasscoe, K. Tiampo, C. Woods, B. Kar, D. Bausch, P. Sharma, M. Zhang, Z. Chen, J. Wang, M. Pierce, G. Schumann, R. Eguchi, 2021, "Integrating Hydrologic Models and Earth Observation Data for Global Flood Forecasting and Alerting." American Society of Photogrammetry and Remote Sensing.`,
          pdf: "#"
        },
        {
          title: `M. Glasscoe, B. Kar, D. Bausch, G. Hempe, C. Chiesa, K. Tiampo, Z. Chen, G. Schumann, R. Eguchi, C. Huyck, M. Pierce, J. Wang. 2020. “Rapid Flood Severity Classification and Alerting for the Spring 2020 Africa Floods: A Case Study.” American Geophysical Union.`,
          pdf: "#"
        },
        {
          title: `C. Woods, K. Tiampo, M. Glasscoe, M. Pierce, B. Kar, D. Bausch, G. Schumann. 2020. “An Automated Approach to Flood Detection Through a Threshold Based Method and Machine Learning using Sentinel-1A/B SAR Data.”American Geophysical Union.`,
          pdf: "#"
        },
        {
          title: `S. Ghosh, C. Huyck, R. Eguchi, M. Glasscoe, B. Kar, K. Tiampo, Z. Chen, D. Bausch. 2020. “Earth Observation (EO) Based Critical Infrastructure Exposure Models and Flood Forecasting Techniques for Risk Monitoring and Management for the City of Vadodara, India.” American Geophysical Union.`,
          pdf: "#"
        },
        {
          title: `Glasscoe et al. (2020) "Advancin Access to Global Flood Modeling and Alerting Using the PDC DisasterAWARE Platform and Remote Sensing Technologies, GFP Virtual Meeting, Flood Forecasting Session.`,
          pdf: "#"
        },
        {
          title: `Molan Zhang and ZhiQiang Chen (2021). "Deep Metric Learning for Disaster Mapping and Damage Identification in Remote Sensing Images". ASCE Lifeline Conference, 2021. ASCE. Los Angeles, CA.`,
          pdf: "#"
        },
        {
          title: `Schumann et al. (2020). “Using a Model-of-Models Approach and Remote Sensing Technologies to Improve Flood Disaster Alerting”. EGU 2020.`,
          pdf: "#"
        },
        {
          title: `Glasscoe et al. (2019) “Advancing Access to Global Flood Modeling and Alerting Using the PDC DisasterAWARE Platform and Remote Sensing Technologies. American Geophysical Union (AGU). San Francisco, CA.`,
          pdf: "#"
        },
        {
          title: `Prativa Sharma, Molan Zhang, ZhiQiang Chen, and Elaina Sutley (2019). “Deep Learning of Tornado Disaster Scenes Using Unmanned-Aerial Vehicle (UAV) Images”. AGU Fall Meeting. San Francisco.https://agu.confex.com/data/handout/agu/fm19/Paper_592329_handout_19644_0.pdf`,
          pdf: "#"
        }
      ],
      mediaReleases: [
        {
          publisher: "PreventionWeb",
          title: "NASA AND PACIFIC DISASTER CENTER PARTNER TO DEVELOP GROUND-BREAKING GLOBAL FLOOD EARLY WARNING SYSTEM",
          link: "https://www.preventionweb.net/news/nasa-and-pacific-disaster-center-partner-develop-ground-breaking-global-flood-early-warning"
        },
        {
          publisher: "PDC | Global",
          title: "NASA and Pacific Disaster Center partner to develop ground-breaking global flood early warning system",
          link: "https://www.pdc.org/nasa-pdc-flood-early-warning-system/"
        },
        {
          publisher: "PDC | Global",
          title: "NASA and Pacific Disaster Center link experts in development of new life-saving technologies",
          link: "https://www.pdc.org/nasa-pdc-develop-life-saving-technologies/"
        }
      ]
    }
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
          Funded by the NASA Disasters Program under its Global Initiative for Flood Forecasting and Alerting (GIFFT),
          Global Flood Map models global flood forecast and inundation information in the world
        </p>
      </div>
    </section>
    <section class="section-2">
      <div>
        <h2 class="row-margin h2-sub"> INTRODUCTION </h2>
        <h2 class="row-margin"> What is Global Flood Map? </h2>
        <p class="row-margin">
          A product of <b>Model of Models (MoM)</b>, an ensemble model, that integrates hydrologic models along with
          earth observation data to forecast flood inundation information globally.
        </p>
        <div style="background: rgba(41, 64, 211, 0.05);padding-top: 30px;padding-bottom: 30px;">
          <h3 class="row-margin">
            <b-icon icon="check-circle"/>
            Using DisasterAWARE to provide flood warnings.
          </h3>
          <p class="row-margin">
            Based on MoM, the new global flood information will reach tens of thousands of disaster management decision
            makers and humanitarian assistance practitioners through <b>PDC’s DisasterAWARE platform</b> as flood
            emergencies unfold. <b>DisasterAWARE® will provide flood early warnings</b> and supplemental advanced
            analytical products to help assess potential impacts.
          </p>
        </div>
      </div>
    </section>
    <section class="section-3">
      <div>
        <h2 class="row-margin h2-sub"> APPROACH </h2>
        <h2 class="row-margin"> Model-of-models approach </h2>
        <p class="row-margin">
          The model-of-models approach combines various flood products from open-source hydrologic models and Earth
          Observation data to determine flood severity risk at sub-watershed level daily and globally. In the current
          version of this model, flood outputs are being leveraged, including:
           
        </p>
        <div class="row-margin d-flex flex-row">
          <div class="w-50">
            <h3>
              <b-icon icon="star-fill"/>
              Forecasting flood severity
            </h3>
            <p>Global Flood Awareness System (GloFAS) and Global Flood Monitoring System (GFMS) data are used to
              forecast flood severity.</p>
          </div>
          <div class="w-50">
            <h3>
              <b-icon icon="star-fill"/>
              Flood severity in near real-time
            </h3>
            <p>MODIS Flood Products from Dartmouth Flood Observatory (DFO/MODIS) and Visible Infrared Imaging Radiometer
              Suite (VIIRS) data are used to determine flood severity in near real-time based on potential
              inundation.</p>
          </div>
        </div>
        <div class="row-margin d-flex flex-row" style="margin-bottom: 20px;">
          <div class="w-50" style="margin-right: 20px;">
            <h3>
              <b-icon icon="star-fill"/>
              Forecasting flood severity from changing tropical storms
            </h3>
            <p>The Hurricane Weather Research and Forecasting (HWRF) model allows forecasting flood severity from
              rapidly changing tropical storm events.</p>
          </div>
          <div class="w-50">
            <h3>
              <b-icon icon="star-fill"/>
              Trigger alert messages via DisasterAWARE
            </h3>
            <p>The flood severity is used to trigger alert messages for high-severity flood events via PDC’s
              DisasterAWARE global platform.</p>
          </div>
        </div>
        <div class="row-margin d-flex flex-row" style="margin-bottom: 20px;">
          <div class="w-50" style="margin-right: 20px;">
            <h3>
              <b-icon icon="star-fill"/>
              Trigger impact assessment
            </h3>
            <p>The flood severity is used to trigger processing of Sentinel 1 (Synthetic Aperture Radar imagery) and
              Sentinel 2 (optical imagery) as well as population and infrastructure data to assess potential impacts of
              flood events.</p>
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
        </div>
      </div>
    </section>

    <section class="section-6" id="section-team">
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

    <section class="section-7">
      <div>
        <h2 class="row-margin h2-sub"> ACHIEVEMENTS </h2>
        <h2 class="row-margin">Publications</h2>
        <div class="row-margin d-flex flex-column">
          <div v-for="(publication, publicationIndex) in publications" :key="publicationIndex">
            <p><small>{{ publication.title }}
              <b-link :href="publication.pdf">
                <b-icon icon="file-earmark-pdf-fill"/>
              </b-link>
            </small></p>
          </div>
        </div>
      </div>
    </section>

    <section class="section-8">
      <div>
        <h2 class="row-margin h2-sub"> ACHIEVEMENTS </h2>
        <h2 class="row-margin">Presentations</h2>
        <div class="row-margin d-flex flex-column">
          <div v-for="(presentation, presentationIndex) in presentations" :key="presentationIndex">
            <p><small>{{ presentation.title }}
              <b-link :href="presentation.pdf">
                <b-icon icon="file-earmark-pdf-fill"/>
              </b-link>
            </small></p>
          </div>
        </div>
      </div>
    </section>

    <section class="section-9">
      <div>
        <h2 class="row-margin h2-sub"> ACHIEVEMENTS </h2>
        <h2 class="row-margin">Media Releases</h2>
        <div class="row-margin d-flex flex-column">
          <div v-for="(mediaRelease, mediaReleaseIndex) in mediaReleases" :key="mediaReleaseIndex">
            <p>
              <strong>{{ mediaRelease.publisher }}</strong>&nbsp;<small>{{ mediaRelease.title }}</small><br/>
              <b-link :href="mediaRelease.link" class="text-secondary">
                {{ mediaRelease.link }}
              </b-link>
            </p>
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

section.section-7 > div {
  padding-top: 50px;
  padding-bottom: 50px;
}

section.section-8 > div {
  padding-top: 50px;
  padding-bottom: 50px;
}

section.section-9 > div {
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
