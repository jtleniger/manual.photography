<template>
  <section class="container">
    <section class="hero is-info">
      <div class="hero-body">
        <h1 class="title">
          Manual Photography
        </h1>
        <h2 class="subtitle">
          Made Simple
        </h2>
      </div>
    </section>
    <section class="section">
      <h1 class="title">
        Basics
      </h1>
      <p>
        A picture is basically capturing light.
      </p>
      <p>
        If you get too much, your picture might look like this:
      </p>
      <div class="overexposed">
        <img src="~/assets/berries.jpg">
      </div>
      <p>
        If you get too little, your picture might look like this:
      </p>
      <div class="underexposed">
        <img src="~/assets/berries.jpg">
      </div>
      <p>
        We don't want that. We're trying to go full goldilocks, so tweak stuff to get it right.
      </p>
    </section>
    <section class="section">
      <h1 class="title">
        Aperture
      </h1>
      <p>
        Aperture is a fancy word for an adjustable hole inside the lens that can open and close. A low number means wide open, like this:
      </p>
      <div class="aperture-container">
        <div class="aperture wide"></div>
      </div>
      <p>
        A high number means narrow, like this:
      </p>
      <div class="aperture-container">
        <div class="aperture narrow"></div>
      </div>
      <p>
        The big hole lets through more light than the small one. If your picture is too dark or too bright, changing this can fix it.
      </p>
    </section>
    <section class="section">
      <h1 class="title">
        Shutter Speed
      </h1>
      <p>
        The shutter is like a opening and closing a door in front of the sensor. The shutter speed is how fast the camera does it.
      </p>
      <section class="section">
        <p>A small number (bottom of the fraction is big) is fast, like this:
        <div class="shutter fast">
          <div class="curtain top"></div>
        </div>
      </section>
      <section class="section">
        <p>A big number (bottom of the fraction is small or the number is more than one) is slow, like this:
        <div class="shutter slow">
          <div class="curtain"></div>
        </div>
      </section>
      <p>
        If the shutter is open for longer, more light gets in. If your picture is too dark or too bright, changing this can fix it.
      </p>
    </section>
    <section class="section">
      <h1 class="title">
        ISO
      </h1>
      <p>

      </p>
    </section>
  </section>
</template>

<style>

.overexposed img {
  filter: brightness(300%);
}

.underexposed img {
  filter: brightness(50%);
}

.aperture-container {
  width: 200px;
  margin: 8px 0;

  position: relative;
}

.aperture {
  border-radius: 100%;
  border: 2px solid #000;

  margin: 0 auto;
}

.aperture.wide {
  width: 200px;
  height: 200px;
}

.aperture.narrow {
  width: 50px;
  height: 50px;
}

.shutter {
  width: 200px;
  height: 200px;
  border: 2px solid #000;
  margin: 8px 0;

  position: relative;

  overflow: hidden;
}

.shutter .curtain {
  animation-duration: 2s;
  animation-iteration-count: infinite;
  width: 200px;
  height: 200px;
  background-color: #000;
  position: absolute;
  left: -2px;
  top: 0px;
}

@keyframes fastShutter {
  from {
    transform: translateY(0);
  }
  10% {
    transform: translateY(-200px);
  }
  20% {
    transform: translateY(0);
  }
  to {
    transform: translateY(0);
  }
}

@keyframes slowShutter {
  from {
    transform: translateY(0);
  }
  10% {
    transform: translateY(-200px);
  }
  56% {
    transform: translateY(-200px);
  }
  66% {
    transform: translateY(0);
  }
  to {
    transform: translateY(0);
  }
}

.fast .curtain {
  animation-name: fastShutter;
}

.slow .curtain {
  animation-name: slowShutter;
}
</style>
