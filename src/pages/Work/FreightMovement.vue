<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <Hero title="Estes Trucking" kicker="Freight Movement Missions For FEMA.">
        <div v-parallax="0.4" class="cover-image hero-background tinted"></div>
      </Hero>

      <Summary
        content="Our client, one of the top 25 carriers in the transportation industry, provides full-service freight transportation and is the largest privately held less-than-truckload (LTL) company in the United States. They are also an active member of Federal Emergency Management Agency (FEMA) missions."
      >
        <Role>
          <li>Java</li>
          <li>Spring</li>
          <li>Application Development</li>
        </Role>
      </Summary>

      <Challenge>
        <h1 class="challenge-header">CHALLENGE</h1>
        <p
          data-aos="fade-up"
          data-aos-duration="600"
          class="text-white"
        >In support of FEMA missions, our client was relying on expensive, restrictive, and under-performing third-party software to manage high-volume freight movement. The application was crashing during active use, hindering ongoing disaster response. These FEMA missions are a major revenue source for our client, and ethically, they client this was no place to compromise on quality. They urgently needed software with high availability, the capacity to handle heavy loads, the ability to provide resource tracking features and timely detailed reports to better manage the overall mission and its resource utilization.</p>
      </Challenge>

      <SolutionHeader>
        <h1 class="section-header solution-header">SOLUTION</h1>
        <p
          data-aos="fade-up"
          data-aos-duration="600"
        >DEPENDABLE WEB APPLICATION FOR DISASTER MANAGEMENT</p>
      </SolutionHeader>

      <Solution>
        <p
          data-aos="fade-up"
          data-aos-duration="600"
        >Our client required a highly available, full featured, highly responsive and scalable enterprise web application to manage and grow their footprint in FEMA missions and thereby significantly increase their annual revenue. Taking into account the client’s existing IT skill set, project timelines and IT investments, Data Concepts proposed the following solution:</p>
        <ul data-aos="fade-up" data-aos-duration="600" data-aos-delay="100">
          <li>- Analyze detailed business requirements to model the current and projected future demands of the FEMA missions.</li>
          <li>- Implement the business needs through a new enterprise web application using Java and latest technologies like Spring MVC, Spring Security, Spring Framework, Maven, OpenJPA, JMS, AJAX, JSP, log4j, PDF and Excel open source frameworks, and WebSphere Distributed Cache.</li>
          <li>- Develop an Application Dashboard with real-time details about each deployed resource.</li>
          <li>- For data privacy, deploy the application using database and application server instance installed in an on-premise infrastructure.</li>
          <li>- Implement Spring Security to manage user authentication and authorization using on-premise Active Directory.</li>
          <li>- Provide high availability and scalability by deploying the web application in a clustered WebSphere v8.0 ND environment installed on Red Hat Enterprise Linux.</li>
          <li>- For deployment automation, use Maven to generate enterprise application archive files and integrate it with Jenkins for build automation and automated deployments to the target application server.</li>
          <li>- Simulate 10 parallel high traffic missions using HP Load Runner to load test the application.</li>
        </ul>
      </Solution>

      <Outcome>
        <h1 class="section-header medium outcome-header">OUTCOME</h1>
        <p
          data-aos="fade-up"
          data-aos-duration="600"
        >With a total development cost of less than one year of the third-party software, Data Concepts developed and rigorously tested the application for our client. The application has been in active use from the last 3 years with virtually no outages. Our client provided a demo of the application to FEMA officials who were impressed with the application and increased their business with our client, preferring them over competitors still utilizing the ineffective third-party software.</p>
      </Outcome>
    </div>
  </div>
</template>

<script>
import NavBarWhite from "../../components/NavBarWhite.vue";
import ModalMenu from "../../components/ModalMenu.vue";
import Hero from "../../components/Hero.vue";
import Summary from "../../components/work/Summary.vue";
import Challenge from "../../components/work/Challenge.vue";
import Role from "../../components/work/Role.vue";
import SolutionHeader from "../../components/work/SolutionHeader.vue";
import Solution from "../../components/work/Solution.vue";
import Outcome from "../../components/work/Outcome.vue";

export default {
  name: "FreightMovement",
  components: {
    NavBarWhite,
    ModalMenu,
    Hero,
    Summary,
    Challenge,
    Role,
    SolutionHeader,
    Solution,
    Outcome
  }
};
</script>


<style lang="sass" scoped>
@import "../../assets/sass/settings.sass"

.hero-background
  background-image: url(../../assets/background/work-large/freight-movement.jpg)
  background-position: center

#first
    background-color: #426EFF

.challenge-header
    font:
        size: 1.8rem
    color: #426EFF
    margin-bottom: 30px

.outcome-header
    font:
        size: 2rem
        weight: 600
    letter-spacing: 4px
    color: #426EFF

.solution-header:after
    background-color: #426EFF

</style>