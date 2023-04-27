<script>
import AppHeader from "../components/AppHeader.vue"
import TM_Bausch_Doug from "../assets/team-members/Bausch_Doug.png"
import TM_Chen_ZQ from "../assets/team-members/Chen_ZQ.png"
import TM_Chiesa_Chris from "../assets/team-members/Chiesa_Chris.jpg"
import TM_Eguchi_Ron from "../assets/team-members/Eguchi_Ron.png"
import TM_Glasscoe_Margaret from "../assets/team-members/Glasscoe_Margaret.jpg"
import TM_Hampe_Greg from "../assets/team-members/Hampe_Greg.jpg"
import TM_Huyck_Charlie from "../assets/team-members/Huyck_Charlie.jpg"
import TM_Kar_Bandana from "../assets/team-members/Kar_Bandana.jpg"
import TM_Pierce_Marlon from "../assets/team-members/Pierce_Marlon.png"
import TM_Dinuka_DeSilva from "../assets/team-members/dinuka_desilva.jpeg"
import TM_Schumann_Guy from "../assets/team-members/Schumann_Guy.jpg"
import TM_Tiampo_Kristy from "../assets/team-members/Tiampo_Kristy.jpg"
import TM_Wang_Jun from "../assets/team-members/Wang_Jun.jpg"
import TM_Prativa_Sharma from "../assets/team-members/Prativa_Sharma.jpg"
import TM_Zhang_Molan from "../assets/team-members/Zhang_Molan.jpg"
import TM_Meyer_Franz from "../assets/team-members/Meyer_Franz.jpg"
import TM_Kennedy_Joseph from "../assets/team-members/Kennedy_Joseph.jpg"
import TM_Schultz_Lori from "../assets/team-members/Schultz_Lori.jpg"
import TM_Melancon_Alexander from "../assets/team-members/Melancon_Alexander.jpg"
import TM_Jo_MinJeong from "../assets/team-members/Jo_MinJeong.jpg"
import TM_Osmanoglu_Batuhan from "../assets/team-members/Osmanoglu_Batuhan.jpg"
import TM_Amyx_Paul from "../assets/team-members/Amyx_Paul.jpg"
import TM_Mendoza_Marina from "../assets/team-members/Mendoza_Marina.jpg"

export default {
  name: "HomeView",
  components: {AppHeader},
  data() {
    return {
      contributors: [
        {name: "Margaret Glasscoe", organization: "University of Alabama in Huntsville", avatarUrl: TM_Glasscoe_Margaret, role: "PI"},
        {name: "Doug Bausch", organization: "Niyam IT/PDC", avatarUrl: TM_Bausch_Doug, role: "MoM"},
        {
          name: "Bandana Kar",
          //organization: "AAAS Science, Technology and Policy Fellow at Department of Energy",
          organization: "Department of Energy",
          avatarUrl: TM_Kar_Bandana, role: "MoM"
        },
        {name: "Marlon Pierce", organization: "Indiana University", avatarUrl: TM_Pierce_Marlon, role: "MoM"},

        {name: "Jun Wang", organization: "Indiana University", avatarUrl: TM_Wang_Jun, role: "MoM"},
        {name: "Guy Schumann", organization: "ImageCat Inc.", avatarUrl: TM_Schumann_Guy, role: "MoM"},
        {name: "Marina Mendoza", organization: "ImageCat Inc.", avatarUrl: TM_Mendoza_Marina, role: "MoM"},
        {name: "Greg Hampe", organization: "University of Hawaii/PDC", avatarUrl: TM_Hampe_Greg, role: "PDC"},
        {name: "Chris Chiesa", organization: "University of Hawaii/PDC", avatarUrl: TM_Chiesa_Chris, role: "PDC"},

        {
          name: "Kristy Tiampo",
          organization: "University of Colorado, Boulder",
          avatarUrl: TM_Tiampo_Kristy,
          role: "Remote Sensing"
        },
        {name: "Franz Meyer", organization: "University of Alaska Fairbanks", avatarUrl: TM_Meyer_Franz, role: "Remote Sensing"},
        {
          name: "Joseph Kennedy",
          organization: "University of Alaska Fairbanks",
          avatarUrl: TM_Kennedy_Joseph,
          role: "Remote Sensing"
        },
        {
          name: "Lori Schultz",
          organization: "NASA Marshall Space Flight Center",
          avatarUrl: TM_Schultz_Lori,
          role: "Remote Sensing"
        },
        {
          name: "Alexander Melancon",
          organization: "University of Alabama in Huntsville",
          avatarUrl: TM_Melancon_Alexander,
          role: "Remote Sensing"
        },
        {
          name: "MinJeong Jo",
          organization: "NASA Goddard Space Flight Center",
          avatarUrl: TM_Jo_MinJeong,
          role: "Remote Sensing"
        },
        {
          name: "Batuhan Osmanoglu",
          organization: "NASA Goddard Space Flight Center",
          avatarUrl: TM_Osmanoglu_Batuhan,
          role: "Remote Sensing"
        },
        {
          name: "ZhiQiang Chen",
          organization: "University of Missouri-Kansas City",
          avatarUrl: TM_Chen_ZQ,
          role: "Remote Sensing"
        },
        {
          name: "Charlie Huyck",
          organization: "ImageCat Inc.",
          avatarUrl: TM_Huyck_Charlie,
          role: "Infrastructure Exposure"
        },
        {name: "Ron Eguchi", organization: "ImageCat Inc.", avatarUrl: TM_Eguchi_Ron, role: "Infrastructure Exposure"},
        {name: "Paul Amyx", organization: "ImageCat Inc.", avatarUrl: TM_Amyx_Paul, role: "Infrastructure Exposure"},
      ],
      students: [
        {name: "Dinuka De Silva", organization: "Indiana University", avatarUrl: TM_Dinuka_DeSilva},
        {name: "Molan Zhang", organization: "University of Missouri Kansas City", avatarUrl: TM_Zhang_Molan}
      ],
      alumnus: [
        {name: "Prativa Sharma", organization: "University of Missouri Kansas City", avatarUrl: TM_Prativa_Sharma}
      ],
      publications: [
        {
          title: `Kar, B., Sharma, P., Chen, Z., Wang, J., Bausch, D., Schumann, G., Pierce, M., Eguchi, R.,Glasscoe, M. An ensemble approach to global flood severity forecasting and alerting in near real-time, Proceedings, International Society for Photogrammetry and Remote Sensing Congress, 2022.`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Andrew Kruczkiewicz, Fabio Cian, Irene Monasterolo, Giuliano Di Baldassarre, Astrid Caldas, Moriah Royz, Margaret Glasscoe, Nicola Ranger and Maarten van Aalst, 2022,  Multiform flood risk in a rapidly changing world: what we do not do, what we should and why it matters, Environ. Res. Lett. 17 081001`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Tiampo, K.F., Huang, L., Simmons, C., Woods, C., Glasscoe, M.T. Detection of flood extent using Sentinel-1A/B synthetic aperture radar: An application for Hurricane Harvey, Houston, TX, Remote Sensing, 14, 2261, doi:10.3390/rs14092261, 2022.`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Kar, B. and Schumann, G. (invited commentary paper). 2022. “Reproducibility and Replicability of Flood Models”, Hydrological Processes Today, 36(9). https://doi.org/10.1002/hyp.14666`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Ghosh, S., Glasscoe, M., Kar, B., Tiampo, K., Green, D., Mendoza, M. and Hyuck, C., 2021. “Detection and Alert for the City of Vadodara: A Space-based Flood Approach for Mitigating Impacts on Critical Infrastructures and Reducing Economic Losses”, Know Disasters, July-August 2021.`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Sharma, P., Wang, J., Zhang, M., Woods, C., Kar, B., Bausch, D., Chen, Z., Tiampo, K., Glasscoe, M., Schumann, G., Pierce, M. and Eguchi, R. 2020. “DisasterAWARE-A Global Alerting Platform for Flood Events”, ISPRS Annals of the Photogrammetry, Remote Sensing and Spatial Information Sciences, VI-3/W1-2020, 107-113. https://doi.org/10.5194/isprs-annals-VI-3-W1-2020-107-2020`,
          pdf: null,
          year: "2020"
        },
        {
          title: `Sharma, P, Kar, B., Wang, J. and Bausch, D. 2021. “A Machine Learning Approach to Flood Severity Classification and Alerting” In Proceedings of 4th ACM SIGSPATIAL International Workshop on Advancements in Resilient and Intelligent Cities. https://doi.org/10.1145/3486626.3493432`,
          pdf: null,
          year: "2021"
        },
        {
          title: `K. Tiampo, C. Woods, L. Huang, P. Sharma, Z. Chen, B. Kar, D. Bausch, C. Simmons, R. Estrada, M. Willis, M. Glasscoe. 2021. “A Machine Learning Approach to Flood Depth and Extent Detection Using Sentinel 1A/B Synthetic Aperture Radar”, In Proceedings of the 2021 IGARSS.`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Kar, B., Bausch, B., Wang, J., Sharma, P., Chen, Z., Schumann, G., Pierce, M., Tiampo, K., Eguchi, R. and Glasscoe, M. 2020. “An Integrated Model of Models for Global Flood Alerting”, WIT Transactions on the Built Environment, 194: 73-86. ISSN# 1743-3509, WIT Press.`,
          pdf: null,
          year: "2020"
        }
      ],
      presentations: [
        {
          title: `Glasscoe, Margaret, Kar, Bandana, Meyer, Franz,  Tiampo, Kristy, Huyck, Charles,  Chiesa, Chris, Hampe, Greg,   Osmanoglu, Batuhan,  Schultz, Lori. 2021, Dissemination of Global Surface Water Mapping from SAR and Optical Data to Global Stakeholders, American Geophysical Union Fall Meeting.`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Ghosh, Shubharoop , Glasscoe, Margaret , Kar, Bandana, Tiampo, Kristy, Huyck, Charles, Hampe, Greg ;, and  Amyx, Paul , 2021, A framework for flood detection and alerting for Vadodara to mitigate impacts on critical infrastructure and reduce economic losses, American Geophysical Union Fall Meeting`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Tiampo, K., Woods, C., Huang, L., Sharma, P., Chen, Z., Kar, B., Bausch, D., Simmons, C., Estrada, R., Willis, M., Glasscoe, M. A Machine Learning Approach to Flood Depth and Extent Detection Using Sentinel 1A/B Synthetic Aperture Radar, oral presentation, IEEE International Geoscience and Remote Sensing Symposium (IGARSS 2021), July 2021.`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Glasscoe, M., Tiampo, K., Woods, C., Kar, B., Bausch, D., Sharma, P., Zhang, M., Chen, Z., Wang, J., Pierce, M., Schumann, G., Eguchi, R., Integrating Hydrologic Models and Earth Observation Data for Global Flood Forecasting and Alerting, ASPRS – IMAGING AND GEOSPATIAL SOCIETY Annual meeting (virtual), 2021.`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Kar, B., Glasscoe, M., Bausch, D., Sharma, P., Wang, J., Schumann, G., Tiampo, K., Chen, Z., Eguchi, R., Pierce, M., 2022, AN ENSEMBLE APPROACH TO GLOBAL FLOOD SEVERITY FORECASTING AND ALERTING IN NEAR REAL-TIME, ISPRS Congress`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Ghosh, S., Glasscoe, M., Kar, B., Tiampo, K., and Huyck, C., 2022, Earth observation (EO) based approaches for developing flood risk products to support mitigation and response activities: A demonstration study for Vadodara, India, IGARSS.`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Kristy Tiampo, Clay Woods, Lingcao Huang, Prativa Sharma, ZhiQiang Chen, Bandana Kar, Doug Bausch, Conor Simmons, Michael Willis, Margaret Glasscoe, 2021. "Advanced Flood Extent Detection Algorithms Applied to Sentinel 1A/B Synthetic Aperture Radar Data." Western-ICLR Multi-hazard Risk and Resilience Workshop, Nov 2021.`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Molan Zhang and ZhiQiang Chen, “Urban Road Network and Flood Damage Assessment using Optical Remote Sensing Data and Deep Metric Learning”. Abstract submit to 2022 DSPS (1st International Data Science for Pavements Symposium)`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Chen, Z., Zhang, M., Glasscoe, M., Tiampo, M. and Kar, B.. 2022. “Resilience Assessment of Urban Road Network with Flood Damage Using Remote Sensing Data,” AGU, Chicago, IL.`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Schumann, G., Glasscoe, M. and Kar, B. 2022. “Global Satellite-based Flood Monitoring Post-MODIS”, LANCE UWG (https://wiki.earthdata.nasa.gov/display/LANCE/LANCE+UWG%3A+3-4+May+2022).`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Ghosh, S., Glasscoe, M., Kar, B., Tiampo, K., Huyck, C., Amyx, P. and Hempe, G. 2022. “Stakeholder Engagement to Disseminate Flood Severity, inundation, and Critical Infrastructure Exposure Information for Mitigation”, ASPRS.`,
          pdf: null,
          year: "2022"
        },
        {
          title: `Sharma, P., Kar, B., Wang J. and Bausch, D.. 2021. “A Machine Learning Approach to Flood Severity Classification and Alerting”, 4th ACM SIGSPATIAL International Workshop on Advancements in Resilient and Intelligent Cities.`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Glasscoe, M., Tiampo, K., Woods, C., Kar, B., Bausch, D., Sharma, P., Zhang, M., Chen, Z., Wang, J., Pierce, M., Schumann, G. and Eguchi. R., 2021 . “Integrating Hydrologic Models and Earth Observation Data for Global Flood Forecasting and Alerting”, American Society of Photogrammetry and Remote Sensing Annul Conference (ASPRS).`,
          pdf: null,
          year: "2021"
        },
        {
          title: `Sharma, P, Zhang, M., Wang, J., Wods, C., Kar, B., Chen, Z., Tiampo, K., Schumann, G., Pierce, M. and Eguchi R. 2020. “DisasterAWARE-A Global Alerting Platform for Flood Events”, GI4DM.`,
          pdf: null,
          year: "2020"
        },
        {
          title: `Glasscoe, M., Kar., B., Bausch, D., Hampe, G., Chisea, C., Tiampo, K., Chen, Z., Schumann, G., Eguchi, R., Huyck, C., Pierce, M. and Wang, J. 2020. “Rapid Flood Severity Classification and Alerting for the Spring 2020 Africa Floods: A Case Study”, AGU.`,
          pdf: null,
          year: "2020"
        },
        {
          title: `Kar, B., Bausch, D., Wang, J., Sharma, P., Chen, Z., Schumann, G., Pierce, M., Tiampo, K., Eguchi, R. and Glasscoe, M. 2020. “An Integrated Model of Models for Global Flood Alerting”, 7th International Conference on Flood and Urban Water Management (FRIAR 2020).`,
          pdf: null,
          year: "2020"
        },
        {
          title: `Schumann, G., Glasscoe, M., Bausch, D., Pierce, M., Wang, J. Chen, Z., Eguchi, R., Huyck, C., Tiampo, K. and Kar, B. 2020. “Using a Model-of-Models Approach and Remote Sensing Technologies to Improve Flood Disaster Alerting”, EGU General Assembly 2020, Virtual, https://doi.org/10.5194/egusphere-egu2020-13113.`,
          pdf: null,
          year: "2020"
        }
      ],
      posters: [
        {
          title: `Ghosh, S., Huyck, C., Eguchi, R., Glasscoe, M., Kar, B., Tiampo, K., Chen, Z. and Bausch, D. 2020. “Earth Observation (EO) Based Critical Infrastructure Exposure Models and Flood Forecasting Techniques for Risk Monitoring and Management for the City of Vadodara, India”, AGU.`,
          pdf: null,
          year: "2020"
        },
        {
          title: `Glasscoe, M., Bausch, D., Tiampo, K., Eguchi, R., Pierce, M., Chen, Z., Kar, B. and Schumann, G. 2019. “Advancing Access to Global Flood Modeling and Alerting Using the PDC DisasterAWARE Platform and Remote Sensing Technologies”, AGU. San Francisco, CA.`,
          pdf: null,
          year: "2019"
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
        <h2 class="row-margin"> Model-of-models</h2>
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
      <div>
        <h2 class="row-margin"> SAR-Based Flood Extent and Depth </h2>
        <p class="row-margin">
          Two techniques will be implemented to determine observed flood information from SAR data:
        </p>
            <p class="row-margin"><b-icon icon="star-fill"/>        
            <strong> HydroSAR</strong> provides information on post-event flood mapping, flood depth estimation and resulting flood severity, using remote sensing-based flood information derived from SAR. 
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            Water depth and extent is also being calculated using <strong>machine learning and thresholding</strong>.  
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            The machine learning and threasholding technique and HydroSAR are being compared and cross-validated in GIFFT. 
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            Triggering of SAR flood extent product generation will use event information provided by MoM severity alerts from PDC 
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            Currently SAR-based surface water extent algorithms are fully implemented and validated in cloud-based platforms 
            </p>
      </div>
      <div>
        <h2 class="row-margin"> Infrastructure and Exposure – The Global Economic Disruption Index</h2>
            <p class="row-margin"><b-icon icon="star-fill"/>        
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            The <strong>GEDI</strong> scale is designed to provide simplified qualitative estimates of the severity of a disaster with regards to the global economy. 
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            <strong>Global economic exposure data</strong> is first generated using classification of various EO datasets to detect areas of critical infrastructure (CI) or industrial activity. The detected areas are assigned economic value based on a global economic input/output model. 
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            <strong>Real-time disaster data</strong> is then applied to the exposure to estimate economic impact, and the result is aggregated to a regional level. 
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            The GEDI score for the disaster is calculated by comparing the pre-event and post-event values for these regional aggregates. 
            </p><p class="row-margin"><b-icon icon="star-fill"/>
            The system is currently being tested using hurricane event data as input. The plan is to expand this to flood events using products derived from the Model of Models process, with eventual dissemination of GEDI results through PDC. 
            </p>
      </div>
      <div>
        <h2 class="row-margin">DisasterAWARE<sup>®</sup></h2>
            <p class="row-margin"><b-icon icon="star-fill"/>        
            Currently, PDC’s <strong>DisasterAWARE</strong> platform incorporates <strong>Model of Models (MoM)</strong> outputs as flood “incidents,” visually depicting potential floods in the context of population and infrastructure that may become affected. Automated procedures have been developed to categorize MoM outputs as DisasterAWARE “hazards,” allowing for their dissemination to users along with other flood products that assess potential impacts.
            </p>
            <p class="row-margin"><b-icon icon="star-fill"/>
              PDC’s stakeholders include UN, DoD, FEMA and their equivalents around the world.  Additionally, the DisasterAWARE platform has 2 million users worldwide and is a fully functional and sustained platform used to disseminate alerts and analytical products for 18 different hazard types.  
            </p>        
      </div>
    </section>
    <section class="section-4">
      <div>
        <h2 class="row-margin h2-sub"> BENEFITS </h2>
        <h2 class="row-margin">Impacts of the Global Flood Map</h2>
        <div class="row-margin d-flex flex-row">
          <div>
            <div class="benefit-icon">
              <img src="../assets/flooded-house-1.png"/>
            </div>
            <h3>Flood extent, depth resolution</h3>
            <p>
              This new technology will be used to create much-needed products that include flood extent and depth at
              finer resolution using Synthetic Aperture Radar (Sentinel 1) data.
            </p>
          </div>

          <div style="margin-left: 20px; margin-right: 20px;">
            <div class="benefit-icon">
              <img src="../assets/mission-1.png"/>
            </div>
            <h3>Anticipate flood impacts</h3>
            <p>
              It will also help anticipate flood impacts on population and critical infrastructures using optical
              imagery as well as geospatial socioeconomic and infrastructure data.
            </p>
          </div>

          <div>
            <div class="benefit-icon">
              <img src="../assets/decision-1.png"/>
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

    <section class="section-6" id="section-team">
      <div>
        <h2 class="row-margin h2-sub"> TEAM </h2>
        <h2 class="row-margin">Contributors</h2>
        <div class="row-margin d-flex flex-row flex-wrap">
          <div v-for="(contributor, contributorIndex) in contributors" :key="contributorIndex"
               style="width: 250px; height: 250px;padding: 10px;" class="text-center">
            <div class="contributor-avatar d-inline-block">
              <img v-if="contributor.avatarUrl" class="w-100" :src="contributor.avatarUrl">
              <img v-else class="w-100" src="../assets/Rectangle-7.png">
            </div>
            <div class="w-100 text-center">
              <h3 class="text-center">{{ contributor.name }}</h3>
              <small class="bg-primary text-light"
                     style="line-height: 18px;font-size: 12px;padding: 2px 10px;display: inline-block;border-radius: 4px;">{{
                  contributor.role
                }}</small>
              <p class="text-center" style="line-height: 16px;font-size: 13px;">{{ contributor.organization }}</p>
            </div>
          </div>
        </div>


        <h2 class="row-margin h2-sub"> TEAM </h2>
        <h2 class="row-margin">Students</h2>
        <div class="row-margin d-flex flex-row flex-wrap">
          <div v-for="(contributor, contributorIndex) in students" :key="contributorIndex"
               style="width: 250px; height: 300px;padding: 10px;" class="text-center">
            <div class="contributor-avatar d-inline-block">
              <img v-if="contributor.avatarUrl" class="w-100" :src="contributor.avatarUrl">
              <img v-else class="w-100" src="../assets/Rectangle-7.png">
            </div>
            <h3 class="text-center">{{ contributor.name }}</h3>
            <p class="text-center">{{ contributor.organization }}</p>
          </div>
        </div>


        <h2 class="row-margin h2-sub"> TEAM </h2>
        <h2 class="row-margin">Alumnus</h2>
        <div class="row-margin d-flex flex-row flex-wrap">
          <div v-for="(contributor, contributorIndex) in alumnus" :key="contributorIndex"
               style="width: 250px; height: 300px;padding: 10px;" class="text-center">
            <div class="contributor-avatar d-inline-block">
              <img v-if="contributor.avatarUrl" class="w-100" :src="contributor.avatarUrl">
              <img v-else class="w-100" src="../assets/Rectangle-7.png">
            </div>
            <h3 class="text-center">{{ contributor.name }}</h3>
            <p class="text-center">{{ contributor.organization }}</p>
          </div>
        </div>
      </div>
    </section>

    <section class="section-5">
      <div>
        <h2 class="row-margin h2-sub"> PROJECT SUPPORT </h2>
        <h2 class="row-margin">Our Partners</h2>
        <div class="row-margin d-flex flex-row">
          <!--          <div>-->
          <!--            <div class="partner-logo">-->
          <!--              <img class="w-100" src="../assets/image-2.png">-->
          <!--            </div>-->
          <!--            <h3>University of Alaska Fairbanks</h3>-->
          <!--          </div>-->
          <!--          <div>-->
          <!--            <div class="partner-logo">-->
          <!--              <img class="w-100" src="../assets/image-3.png">-->
          <!--            </div>-->
          <!--            <h3>Marshall Space Flight Center</h3>-->
          <!--          </div>-->
          <!--          <div>-->
          <!--            <div class="partner-logo">-->
          <!--              <img class="w-100" src="../assets/image-4.png">-->
          <!--            </div>-->
          <!--            <h3>Goddard Space Flight Center</h3>-->
          <!--          </div>-->


          <div>
            <div class="partner-logo">
              <img class="w-100" src="../assets/partners/pdc.svg">
            </div>
            <h3>Pacific Disaster Center</h3>
          </div>

          <div>
            <div class="partner-logo">
              <img class="w-100" src="../assets/partners/noaa.png">
            </div>
            <h3>National Oceanic and Atmospheric Administration</h3>
          </div>

          <div>
            <div class="partner-logo">
              <img class="w-100" src="../assets/partners/ceos.png">
            </div>
            <h3>Committee on Earth Observation Satellites</h3>
          </div>

          <div>
            <div class="partner-logo">
              <img class="w-100" src="../assets/partners/un.png">
            </div>
            <h3>United Nations</h3>
          </div>

        </div>
      </div>
    </section>

    <section class="section-7" id="section-presentations-and-publications">
      <div>
        <h2 class="row-margin h2-sub"> ACHIEVEMENTS </h2>
        <h2 class="row-margin">Publications</h2>
        <div class="row-margin d-flex flex-column">
          <div v-for="(publication, publicationIndex) in publications" :key="publicationIndex">
            <p><small>{{ publication.title }}
              <b-link :href="publication.pdf" v-if="publication.pdf">
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
              <b-link :href="presentation.pdf" v-if="presentation.pdf">
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
        <h2 class="row-margin">Posters</h2>
        <div class="row-margin d-flex flex-column">
          <div v-for="(poster, posterIndex) in posters" :key="posterIndex">
            <p><small>{{ poster.title }}
              <b-link :href="poster.pdf" v-if="poster.pdf">
                <b-icon icon="file-earmark-pdf-fill"/>
              </b-link>
            </small></p>
          </div>
        </div>
      </div>
    </section>

    <section class="section-10">
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
  background-image: url("../assets/image2.png");
}

section.section-2 {
  background-image: url("../assets/image1.png");
}

section.section-3 {
  background-image: url("../assets/Rectangle-5.png");
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
  height: 150px;
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
  line-height: 15px;
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
