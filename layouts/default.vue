<template>
    <div>
        <nav class="navbar is-dark" role="navigation" aria-label="main navigation">
            <div class="navbar-brand">
                <a class="navbar-item brand" href="https://tldr.photography">
                    TL;DR
                </a>

                <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false"
                    @click="showNav = !showNav" :class="{ 'is-active': showNav }"
                    data-target="navbar">
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                </a>
            </div>

            <div id="navbar" class="navbar-menu" :class="{ 'is-active': showNav }">
                <div class="navbar-start">
                    <nuxt-link to="/" class="navbar-item">
                        Basics
                    </nuxt-link>

                    <div class="navbar-item has-dropdown is-hoverable">
                        <a class="navbar-link">
                        More
                        </a>

                        <div class="navbar-dropdown">
                            <!-- <nuxt-link to="/aperture" class="navbar-item">
                                Aperture
                            </nuxt-link>
                            <nuxt-link to="/iso" class="navbar-item">
                                ISO
                            </nuxt-link>
                            <nuxt-link to="/shutter-speed" class="navbar-item">
                                Shutter Speed
                            </nuxt-link>
                            <nuxt-link to="/focal-length" class="navbar-item">
                                Focal Length
                            </nuxt-link>

                            <hr class="navbar-divider"> -->

                            <nuxt-link to="/contact" class="navbar-item">
                                Contact
                            </nuxt-link>
                        </div>
                    </div>
                </div>
            </div>
        </nav>
        <nuxt />
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
    </div>
</template>

<script>
export default {
    data() {
        return {
            showNav: false
        }
    },
    watch: {
        '$route' () {
            this.showNav = false;
        }
  }
}
</script>


<style>
a.brand {
    text-transform: uppercase;
    font-weight: bold;
    font-size: 2rem;
}
</style>
