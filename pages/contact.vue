<template>
    <section class="container">
        <section class="section">
            <form name="contact" method="POST" data-netlify-recaptcha="true" data-netlify="true" action="/thankyou">
                <div class="field">
                    <label class="label">Name</label>
                    <div class="control">
                        <input class="input" type="text" name="name" placeholder="Name">
                    </div>
                </div>

                <div class="field">
                    <label class="label">Email</label>
                    <div class="control">
                        <input class="input" type="email" name="email" placeholder="Email">
                    </div>
                </div>

                <div class="field">
                    <label class="label">Message</label>
                    <div class="control">
                        <textarea class="textarea" name="message" placeholder="Message"></textarea>
                    </div>
                </div>

                <div class="field">
                    <div data-netlify-recaptcha="true"></div>
                </div>

                <input type="hidden" name="form-name" value="contact" />

                <div class="field is-grouped">
                    <div class="control">
                        <button type="submit" class="button is-link">Submit</button>
                    </div>
                    <div class="control">
                        <button type="reset" class="button is-text">Clear</button>
                    </div>
                </div>
            </form>
        </section>
    </section>
</template>
