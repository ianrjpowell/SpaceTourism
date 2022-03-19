<template>
  <div class="home">
    <div class="content-container">
      <h2 class="home__lead">So, you want to travel to</h2>
      <h1 class="home__headline">Space</h1>
      <p class="home__text">
        Let's face it; if you want to go to space, you might as well genuinely go
        to outer space and not hover kind of on the edge of it. Well sit back, and
        relax because we'll give you a truly out of this world experience!
      </p>
      <a class="home__cta" href="/Destination">Explore</a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.home {
  height: 100vh;
  background: url("../assets/home-bg-m.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  padding-top: 112px;
  color: #D0D6F9;
  text-align: center;
  font-family: 'Barlow';

  &__lead, &__headline {
    text-transform: uppercase;
  }

  &__lead {
    letter-spacing: 3px;
    margin-bottom: 16px;
  }

  &__headline {
    color: #fff;
    font-size: 80px;
    line-height: 100px;
    font-family: "Bellefair";
    margin-bottom: 16px;
  }

  &__text {
    font-size: 15px;
    line-height: 25px;
    margin-bottom: 81px;
  }

  &__cta {
    width: 150px;
    height: 150px;
    display: block;
    margin: 0 auto;
    color: #0B0D17;
    font-family: 'Bellefair';
    font-size: 20px;
    border-radius: 100%;
    background: #fff;
    text-decoration: none;
    display: flex;
    align-items: center;
    justify-content: center;
    text-transform: uppercase;
    letter-spacing: 1.25px;
  }
}

.content-container {
  padding: 0 24px;
}
</style>