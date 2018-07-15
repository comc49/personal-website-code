<template>
  <section class="homepage">
    <section class="homepage--landing hp-section">
      <section class="homepage--landing--texts fade-in">
        <h2 class="name left-pad">Brian Koo</h2>
        <h1 class="position-title left-pad">FRONT-END DEVELOPER</h1>
        <p class="description left-pad">
          I specialize in building rich interactive web applications
        </p>
      </section>
    </section>
    <section class="homepage--about hp-section">
      <section class="text-section homepage--about--texts fade-in">
        <div class="title">
          <h1 class="section-name">ABOUT</h1>
          <i class="material-icons title-icon">person</i>
        </div>
        <div class="desc about">
          <h1>BRIAN KOO</h1>
          <p class="about-text1">
            Offering experiences of the latest front-end frameworks.
            I am very flexible to meet your needs!
            I write in JavaScript, HTML, CSS, and Python. I like working on scalability,
            performance, reusability, and great user experiences.
          </p>
          <p class="about-text2">
            As a front-end developer with a computer science degree,
            I write code that conforms to the industry standards and follows the best practices for performance.
          </p>
        </div>
      </section>
    </section>
    <section class="homepage--experience hp-section">
      <section class="text-section homepage--experience--texts fade-in">
        <div class="title">
          <h1 class="section-name">EXPERIENCE</h1>
          <i class="material-icons title-icon">list_alt</i>
        </div>
        <section class="desc">
          <div class="work-exp">
            <h1 class="company">BrickSimple LLC</h1>
            <a href="http://bricksimple.com/" target="_blank"><i class="material-icons link">link</i></a>
            <h3 class="duration">Jun 2017 - Present</h3>
            <h2 class="position">Web Application Developer</h2>
          </div>
          <div class="work-exp">
            <h1 class="company">Airborne Interactive</h1>
            <a href="http://airborneinteractive.com/" target="_blank"><i class="material-icons link">link</i></a>
            <h3 class="duration">Feb 2015 - Jul 2016</h3>
            <h2 class="position">Junior Application Developer</h2>
          </div>
          <div class="work-exp">
            <h1 class="company">UCR C&C</h1>
            <a href="http://cnc.ucr.edu/" target="_blank"><i class="material-icons link">link</i></a>
            <h3 class="duration">May 2013 - Sep 2014</h3>
            <h2 class="position">Student Programmer</h2>
          </div>
        </section>
      </section>
    </section>
    <section class="homepage--skillset hp-section">
      <section class="text-section homepage--skillset--texts fade-in">
        <div class="title">
          <h1 class="section-name blue">SKILLSET</h1>
          <i class="material-icons title-icon blue">create</i>
        </div>
        <div class="desc skills blue">
          <div class="skill">HTML5</div>
          <div class="skill">CSS3</div>
          <div class="skill">SASS</div>
          <div class="skill">Javascript</div>
          <div class="skill">Reactjs</div>
          <div class="skill">Angular</div>
          <div class="skill">Vuejs</div>
          <div class="skill">Django</div>
          <div class="skill">Firebase</div>
          <div class="skill">Redux</div>
        </div>
      </section>
    </section>
    <section class="homepage--education hp-section">
      <section class="text-section homepage--education--texts fade-in">
        <div class="title">
          <h1 class="section-name">EDUCATION</h1>
          <i class="material-icons title-icon">school</i>
        </div>
        <div class="education-desc desc">
          <h3 class="year pd-b">2014</h3>
          <h1 class="degree pd-b">Computer Science</h1>
          <h2 class="university pd-b">University Of California Riverside</h2>
        </div>
      </section>
    </section>
    <!-- <section class="homepage--projects hp-section">
      <section class="text-section homepage--projects--texts fade-in">
        <div class="title">
          <h1 class="section-name blue">PROJECTS</h1>
          <i class="material-icons title-icon blue">build</i>
        </div>
      </section>
    </section> -->
    <section class="homepage--social-media hp-section blue">
      <section class="text-section homepage--social-media--texts fade-in">
        <div class="title">
          <h1 class="section-name">HIT ME UP!</h1>
          <i class="material-icons title-icon contact-icon">contact_mail</i>
        </div>
        <div class="desc">
          <a href="https://www.github.com/comc49" target="_blank">
            <i class="fab social-icon fa-github"></i>
          </a>
          <a href="https://www.linkedin.com/in/koobrian" target="_blank">
            <i class="fab social-icon fa-linkedin"></i>
          </a>
          <a href="https://www.codepen.io/comc49" target="_blank">
            <i class="fab social-icon fa-codepen"></i>
          </a>
        </div>
      </section>
    </section>
  </section>
</template>

<script>
export default {
  name: 'Homepage',
  data() {
    return {
      test: 'test',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import "../assets/scss/classes";
  .homepage {
    box-sizing: border-box;
    grid-area: main;
    &--landing {
      background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);
      height: 100vh;
      &--texts {
        opacity: 0;
        margin-left: 10vw;
        &.fade-in {
          opacity: 1;
          animation-name: fadeInOpacity;
          animation-iteration-count: 1;
          animation-timing-function: ease-in;
          animation-duration: 2s;
        }
        @keyframes fadeInOpacity {
          0% {
            opacity: 0;
          }
          100% {
            opacity: 1;
          }
        }

        .name , .description {
          font-size: 2rem;
          color: #deeef5;
        }
        .name {
          padding-top: 2rem;
          margin-bottom: 30vh;
        }
        .description {
          padding-top: 1rem;
          padding-right: 1rem;
        }
        .position-title {
          font-size: calc(3rem + 1vw);
          padding-right: 1rem;
          &:after {
            content: ' ';
            display: block;
            width: 50px;
            border: 2px solid #fff;
          }
        }
      }
    }
    &--about {
      color: #258def;
      height: 100%;
      &--texts {
        display: flex;
      }
      .about {
        color: #5d748c;
        font-size: 1.5rem;
        padding-right: 2rem;
        padding-bottom: 2rem;
      }
      .about-text1 {
        margin-bottom: 3rem;
      }
      .about-text1, .about-text2 {
        padding-right: 4rem;
      }
    }
    &--experience {
      background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);

      .work-exp {
        &:nth-child(n+2) {
          margin-top: 2rem;
        }
      }
      .link {
        display: inline-block;
        padding: 0 .5rem;
        font-size: 1.5rem;
      }

      .company {
        display: inline-block;
        font-size: 2rem;
      }
      .position, .duration {
        color: #deeef5;
      }
    }
    &--skillset {
      .desc {
        display: flex;
        flex-wrap: wrap;
      }
      .skill {
        display: flex;
        justify-content: center;
        font-size: 1.5rem;
        border: 2px solid;
        width: 125px;
        padding: .5rem;
        margin: .5rem;
        border-radius: 25px;
      }
    }
    &--education {
      background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);
      .education-desc {
          padding-bottom: 1rem;
      }
      .year {
        color: #deeef5;
      }
    }
    // &--projects {
    // }
    &--social-media {
      //background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);
      .social-icon {
        font-size: 3rem;
        margin-right: 1rem;
        padding: .5rem;
      }
      .desc {
        display: flex;
        justify-content: center;
      }
      .title {
        .title-icon.contact-icon {
          margin-left: 0;
        }
      }

    }
    .hp-section {
      width: 100vw;
    }
    @media (max-width: 750px) {
      .text-section {
        flex-direction: column;
        align-items: center;
      }
      .title {
        display: flex;
        flex-direction: column;
        align-items: center;
      }
      .skill {
        font-size: 1rem;
        width: 80px;

      }
      .desc {
        display: flex;
        flex-direction: column;
        text-align: center;
        align-items: center;
        padding-top: 2rem;
        &.about {
          padding: 0;
        }
        .about-text1, .about-text2 {
          padding: 0;
        }
      }
      .work-exp {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
      }
      .skills {
        flex-direction: row;
        justify-content: center;
      }
      .year, .degree, .university {
        display: flex;
        justify-content: center;
      }
      .section-name {
        text-align: center;
        &::after {
          width: 100% !important;
        }
      }
      .social-icon {
        margin: 0;
      }

    }
    .text-section {
      display: flex;
      padding-left: 3vw;
      padding-top: 3rem;
      padding-bottom: 3rem;

      .title {
        width: 35vw;
        letter-spacing: 2px;
        .section-name {
          font-size: 2rem;
          &:after {
            content: ' ';
            display: block;
            width: 50px;
            border: 2px solid;
            margin-top: .5rem;
          }
        }
      }
      .title-icon {
        margin-top: 1rem;
        margin-left: -.5rem;
        font-size: 4rem;
      }
      .desc {
        width: 65vw;
      }
    }
    color: white;

  }
</style>
