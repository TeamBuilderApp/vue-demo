<template>
  <div class="home">
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">{{ heading }}</h1>
          <div class="is-two-thirds column is-paddingless">
            <h2 class="subtitle is-4">{{ subheading }}</h2>
          </div>
          <a class="button is-large is-primary" id="learn">Learn more</a>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <div class="columns pd is-desktop">
          <div class="column is-1 has-text-centered">
            <i class="fa fa-cog is-primary"></i>
          </div>
          <div class="column is-one-third-desktop">
            <p class="title">
              <strong
                >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna
                aliqua.</strong
              >
            </p>
          </div>
          <div class="column">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
          </div>
        </div>
      </div>

      <div class="columns pd">
        <div class="column">
          <div class="card">
            <div class="card-content">
              <p class="title">
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat."
              </p>
              <p class="subtitle">- Classical Latin literature from 45 BC</p>
            </div>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <div class="card-content">
              <p class="title">
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat."
              </p>
              <p class="subtitle">- Classical Latin literature from 45 BC</p>
            </div>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <div class="card-content">
              <p class="title">
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat."
              </p>
              <p class="subtitle">- Classical Latin literature from 45 BC</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      heading: "Vue.js Demo",
      subheading:
        "Vue.js is an open-source, progressive JavaScript framework for building user interfaces and single-page applications.",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "../assets/mediaQuery.scss";

.hero {
  background: url("../assets/clouds2.png");
  background-size: cover;

  .title {
    @include mobile {
      font-weight: bold;
    }
    @include tablet {
      font-size: 2.5rem;
    }
    @include desktop {
      font-size: 4rem;
      margin-top: 2rem;
    }
  }
}
h2 {
  margin: 1.5rem 0 2rem 0 !important;
}
.fa-cog {
  font-size: 40px;
}
#learn {
  @include desktop {
    margin-bottom: 2rem;
  }
}
.pd {
  @include tablet {
    padding: 2em 0;
  }
}
</style>
