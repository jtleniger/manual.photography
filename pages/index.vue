<template>
  <section class="container">
    <section class="hero is-success">
      <div class="hero-body">
        <h1 class="title">
          Manual Photography
        </h1>
        <h2 class="subtitle">
          TL;DR
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
        <img src="~/assets/berries.jpg" alt="Photo of Berries">
      </div>
      <p>
        If you get too little, your picture might look like this:
      </p>
      <div class="underexposed">
        <img src="~/assets/berries.jpg" alt="Photo of Berries">
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
        Aperture is a fancy word for an adjustable hole inside the lens that can open and close. A low number means wide open:
      </p>
      <div class="aperture-container">
        <div class="aperture wide"></div>
      </div>
      <p>
        A high number means narrow:
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
      <p>A small number (bottom of the fraction is big) is fast:
      <div class="shutter fast">
        <div class="curtain top"></div>
      </div>
      <p>A big number (bottom of the fraction is small or the number is more than one) is slow:
      <div class="shutter slow">
        <div class="curtain"></div>
      </div>
      <p>
        If the shutter is open for longer, more light gets in. If your picture is too dark or too bright, changing this can fix it.
      </p>
    </section>
    <section class="section">
      <h1 class="title">
        ISO
      </h1>
      <p>
        ISO is basically a digital volume knob for the camera. It's kind of like turning up the brightness on your phone. If you're picture is too dark or too bright, changing this can fix it.
      </p>
    </section>
    <section class="section">
      <h1 class="title">
        But wait! Why can't this be automatic?
      </h1>
      <p>
        Each of these settings affect the picture, so you gotta juggle them.
      </p>
    </section>
    <section class="section">
      <div class="tile is-ancestor">
        <div class="tile is-parent">
          <article class="tile is-child notification is-primary">
            <p class="title">Aperture</p>
            <p class="subtitle">Make it fancy</p>
            <div class="content">
              <p>
                In addition to light, aperture affects your "depth-of-field", which is a fancy way to say how much stuff is in focus.
              </p>
              <p>
                A big aperture (small f number) means the depth-of-field is <em>shorter</em>. Stuff behind and in front of your focus point will be blurry.
                A small aperture makes the depth-of-field longer, so only stuff really far away from your focus point (close to you and in the distance) is blurry.
              </p>
              <p>
                In a portrait, you might want a blurry background, in a landscape, you may not.
              </p>
            </div>
          </article>
        </div>
        <div class="tile is-parent">
          <article class="tile is-child notification is-info">
            <p class="title">Shutter Speed</p>
            <p class="subtitle">Make it blurry</p>
            <div class="content">
              <p>
                If something in the picture is moving or your hands are shaky, too long of a shutter speed means a blurry picture. Simple enough.
              </p>
              <p>
                This can be used for effect with a tripod if you want smooth water or clouds.
              </p>
            </div>
          </article>
        </div>
        <div class="tile is-parent">
          <article class="tile is-child notification is-warning">
            <p class="title">ISO</p>
            <p class="subtitle">Make it noisy</p>
            <div class="content">
              <p>
                ISO adds noise. That's pretty much the only effect. The higher the number, dark areas look more and more like this:
              </p>
              <img src="~/assets/noisy-berries.jpg" alt="Noisy photo of Berries">
            </div>
          </article>
        </div>
      </div>
    </section>
    <section class="section">
      <h1 class="title">
        How do I know if I've got it right?
      </h1>
      <p>
        Most mirrorless and DSLR cameras with manual mode have an exposure meter that looks something like this:
      </p>
      <img src="~/assets/exposure.svg" alt="Exposure Meter">
      <p>
        Tweak your settings to get the those little tick tacks below the scale near the 0 and you're good to go.
      </p>
    </section>
    <section class="section">
      <h1 class="title">
        That's it.
      </h1>
      <p>
        That's pretty much all you need to know about manual. Better than hours of convoluted YouTube videos and ad-ridden articles, right?
      </p>
      <p>
        The only hard part is using these settings to get the result you want.
      </p>
    </section>
    <footer class="footer">
      <div class="content has-text-centered">
        &copy; {{ new Date().getFullYear() }}, Justin Leniger
      </div>
    </footer>
  </section>
</template>

<style>

img {
  margin: 8px 0;
}

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
