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
      <h1 class="title">What to Tweak</h1>
      <section class="section tight">
        <h1 class="title is-size-4">
          Aperture
        </h1>
        <p>
          Aperture is a fancy word for an adjustable hole inside the lens.
        </p>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <div class="tile is-child example">
              <p class="has-text-centered">
                A low number (like f1.8) means wide open:
              </p>
              <div class="aperture-container">
                <div class="aperture wide"></div>
              </div>
            </div>
          </div>
          <div class="tile is-parent">
            <div class="tile is-child example">
              <p class="has-text-centered">
                A high number (like f22) means narrow:
              </p>
              <div class="aperture-container">
                <div class="aperture narrow"></div>
              </div>
            </div>
          </div>
        </div>
        <p>
          A big hole lets through more light than the small one. If your picture is too dark or too bright, changing this can fix it.
        </p>
      </section>
      <section class="section tight">
        <h1 class="title is-size-4">
          Shutter Speed
        </h1>
        <p>
          The shutter basically passes an opening in front of the sensor. The shutter speed is how fast the camera does it.
        </p>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <div class="tile is-child example">
              <p class="has-text-centered">A small number (like 1/1000s) is fast:
              <div class="shutter fast">
                <div class="curtain">
                  <div class="top"></div>
                  <div class="middle"></div>
                  <div class="bottom"></div>
                </div>
              </div>
            </div>
          </div>
          <div class="tile is-parent">
            <div class="tile is-child example">
              <p class="has-text-centered">A big number (like 1s) is slow:
              <div class="shutter slow">
                <div class="curtain">
                  <div class="top"></div>
                  <div class="middle"></div>
                  <div class="bottom"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <p>
          If the shutter is open for longer, more light gets in. If your picture is too dark or too bright, changing this can fix it.
        </p>
      </section>
      <section class="section tight">
        <h1 class="title is-size-4">
          ISO
        </h1>
        <p>
          ISO is basically a digital volume knob for the camera. It's kind of like turning up the brightness on your phone.
          If your picture is too dark or too bright, changing this can fix it.
        </p>
      </section>
    </section>
    <section class="section">
      <h1 class="title">
        How do I know if I've gotten it right?
      </h1>
      <p>
        Most mirrorless and DSLR cameras with manual mode have a thing on the screen or viewfinder that looks something like this:
      </p>
      <img class="meter" src="~/assets/exposure.svg" alt="Exposure Meter">
      <p>
        Tweak your settings to get the those little tick tacks below the scale near the 0, and then snap a photo.
      </p>
    </section>
    <section class="section">
      <h1 class="title">
        But wait! Why would I want to set these myself?
      </h1>
      <p>
        Each of these settings has its own effect the picture, so if you successfully juggle them, you can control those effects.
      </p>
    </section>
    <section class="section tight">
      <div class="tile is-ancestor">
        <div class="tile is-parent">
          <article class="tile is-child notification is-primary">
            <p class="title">Aperture</p>
            <p class="subtitle">Make It Fancy or Make It Crisp</p>
            <div class="content">
              <p>
                In addition to light, aperture affects your "depth-of-field", which is a fancy way to say how much stuff is in focus.
              </p>
              <p>
                Depth of field is like taking a giant slice of cake out of the space in front of you. Stuff in that slice is sharp.
              </p>
              <p>
                A big hole means the slice of cake is <em>shorter</em>. Stuff behind and in front of your focus point will be blurry.
              </p>
              <img src="~/assets/f1_8.jpg" alt="f1.8">
              <p>
                A small hole makes the slice of cake very <em>long</em>, so almost everything is in focus.
              </p>
              <img src="~/assets/f22.jpg" alt="f22">
              <p>
                In a portrait, you might want a blurry background, so you would use a big hole (large aperture, small number).
                In a landscape, you may not, so you would use a small hole (small aperture, big number).
              </p>
            </div>
          </article>
        </div>
      </div>
      <div class="tile is-ancestor">
        <div class="tile is-parent">
          <article class="tile is-child notification is-info">
            <p class="title">Shutter Speed</p>
            <p class="subtitle">Don't Make It Blurry</p>
            <div class="content">
              <p>
                If something in the picture is moving or your hands are shaky, too long of a shutter speed means a blurry picture.
                Simple enough.
              </p>
              <p>
                Generally, you'll want to keep this as fast (low number) as possible to minimize blur.
              </p>
              <p>
                The shutter speed can be used for effect if you've got a tripod. Leave it open for days to get smooth water or clouds.
              </p>
            </div>
          </article>
        </div>
        <div class="tile is-parent">
          <article class="tile is-child notification is-warning">
            <p class="title">ISO</p>
            <p class="subtitle">Don't Make It Noisy</p>
            <div class="content">
              <p>
                ISO adds noise. That's pretty much the only effect.
                This one is usually used to compensate when you can't tweak the others more.
                The higher the number, dark areas look more and more like this:
              </p>
              <img src="~/assets/noisy-berries.jpg" alt="Noisy photo of Berries">
            </div>
          </article>
        </div>
      </div>
    </section>
    <section class="section">
      <h1 class="title">
        That's it.
      </h1>
      <p>
        That's pretty much all you need to know about manual.
        Better than hours of convoluted YouTube videos and ad-ridden articles, right?
      </p>
      <p>
        The only hard part is using these settings to get the result you want.
      </p>
    </section>
    <footer class="footer">
      <div class="content has-text-centered">
        <p>&copy; {{ new Date().getFullYear() }}, Justin Leniger</p>
        <p>If you found this helpful and are feeling generous, help me pay for the site:</p>
        <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
          <input type="hidden" name="cmd" value="_donations" />
          <input type="hidden" name="business" value="WBYXJZMKLXWEJ" />
          <input type="hidden" name="item_name" value="Hosting / Domain Costs" />
          <input type="hidden" name="currency_code" value="USD" />
          <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" border="0" name="submit"
            title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button" />
          <img alt="" border="0" src="https://www.paypal.com/en_US/i/scr/pixel.gif" width="1" height="1" />
        </form>
      </div>
    </footer>
  </section>
</template>

<style>
p {
  margin: 8px 0;
}

img {
  margin: 8px auto;
  display: block;
}

.section.tight {
  padding: .5rem .5rem;
}

.overexposed img {
  filter: brightness(300%);
}

.underexposed img {
  filter: brightness(30%);
}

.aperture-container {
  width: 220px;
  height: 220px;
  border-radius: 100%;
  margin: 8px auto;
  border: 2px solid #000;

  position: relative;

  background-color: #212121;
}

.aperture {
  border-radius: 100%;
  border: 2px solid #000;
  background-color: white;
  position: absolute;
  top: 50%;
  left: 50%;
}

.aperture.wide {
  width: 180px;
  height: 180px;
  margin: -90px 0 0 -90px;
}

.aperture.narrow {
  width: 30px;
  height: 30px;
  margin: -15px 0 0 -15px;
}

.shutter {
  width: 200px;
  height: 200px;
  border: 2px solid #000;
  margin: 8px auto;

  position: relative;

  overflow: hidden;

  background-image: url('~assets/deer.jpg');
}

.shutter .curtain {
  animation-duration: 5s;
  animation-iteration-count: infinite;
  width: 200px;
  height: 600px;
  position: absolute;
  left: -2px;
  top: -402px;
}

.shutter .curtain .top,.middle,.bottom {
  height: 200px;
}

.shutter .curtain .middle {
  background: transparent;
}

.shutter .curtain .top,.bottom {
  background-color: #212121;
}

.shutter .curtain .top {
  border-bottom: 2px solid #000;
}

.shutter .curtain .bottom {
  border-top: 2px solid #000;
}

@keyframes fastShutter {
  from {
    transform: translateY(0);
  }
  15% {
    transform: translateY(400px);
  }
  to {
    transform: translateY(400px);
  }
}

@keyframes slowShutter {
  from {
    transform: translateY(0);
  }
  50% {
    transform: translateY(400px);
  }
  to {
    transform: translateY(400px);
  }
}

.fast .curtain {
  animation-name: fastShutter;
}

.slow .curtain {
  animation-name: slowShutter;
}

img.meter {
  margin: 24px auto;
}
</style>
