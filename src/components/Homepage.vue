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
          <i class="material-icons person">person</i>
        </div>
        <div class="desc">

        </div>

      </section>
    </section>
    <section class="homepage--experience hp-section">
      <section class="text-section homepage--experience--texts fade-in">
        <div class="title">
          <h1 class="section-name">EXPERIENCE</h1>
          <i class="material-icons person">list_alt</i>
        </div>

      </section>
    </section>
    <section class="homepage--skillset hp-section">
      <section class="text-section homepage--skillset--texts fade-in">
        <div class="title">
          <h1 class="section-name blue">SKILLSET</h1>
          <i class="material-icons icon blue">create</i>
        </div>

      </section>
    </section>
    <section class="homepage--education hp-section">
      <section class="text-section homepage--education--texts fade-in">
        <div class="title">
          <h1 class="section-name">EDUCATION</h1>
          <i class="material-icons">school</i>
        </div>

      </section>

    </section>
    <section class="homepage--projects hp-section">
      <section class="text-section homepage--projects--texts fade-in">
        <div class="title">
          <h1 class="section-name blue">PROJECTS</h1>
          <i class="material-icons icon blue">build</i>
        </div>

      </section>

    </section>
    <section class="homepage--social-media hp-section">
      <section class="text-section homepage--social-media--texts fade-in">
        <div class="title">
          <h1 class="section-name">HIT ME UP!</h1>
          <i class="material-icons person">contact_mail</i>
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
    grid-area: main;
    &--landing {
      background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);
      &--texts {
        opacity: 0;
        margin-left: 7vw;
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
          margin-bottom: 20vh;
        }
        .description {
          padding-top: 1rem;
        }
        .position-title {
          font-size: 4rem;
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
      .text-section {
        padding-left: 5vw;
      }
      .person {
        font-size: 4rem;
        padding: 0;
        margin: 0 -1rem;
      }
    }
    &--experience {
      background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);

    }
    // &--skillset {
    // }
    &--education {
      background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);
    }
    // &--projects {
    // }
    &--social-media {
      background: linear-gradient(to bottom, #007CE9 0%, #70BBFC 100%);
    }
    .hp-section {
      height: 100vh;
      width: 100vw;
    }
    .title {
      .section-name {
        padding-top: 2vw;
        font-size: 2rem;
        &:after {
          content: ' ';
          display: block;
          width: 50px;
          border: 2px solid;
        }
      }
    }
    color: white;

  }
</style>
