<template>
    <b-container fluid id="contact">
        <b-row>
            <b-col sm="12" md="7">
                <h2>{{title}}</h2>
                <p>Dae Yen Sa holds traditional Korean Buddhist celebrations and ceremonies throughout the year. All are invited to attend and participate. To receive regular information and announcements about events and programs please contact us.</p>
                <p><a href="mailto:daeyensatemple@gmail.com">daeyensatemple@gmail.com</a></p>
            </b-col>
            <b-col sm="12" md="5">
                <p>댸연불보정사 <br>
                    케네티컷 ~ 성역 관음성지 <br>
                    <address>
                        Dae Yen Sa International Temple <br>
                        and Meditation Center <br>
                        19 Kinsey Road<br>
                        New Hartford, CT 06057<br>
                        <a class="phone" href="tel:860-489-3254">860-489-3254</a>
                    </address>
                </p>
                <div class="map">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2972.7000144763215!2d-73.05270148467247!3d41.83475737610473!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89e7a18675dc1f8f%3A0x60dd3b8451837d31!2sdae+yen+sa!5e0!3m2!1sen!2sus!4v1551286178456" width="100%" height="100%" frameborder="0" style="border:0" allowfullscreen></iframe>
                </div>
            </b-col>
        </b-row>
        <b-row>
            <b-col sm="12" md="7">
                <h3>Sign up for our newsletter!</h3>
                <!-- Begin Mailchimp Signup Form -->
                <div id="mc_embed_signup">
                    <form action="https://facebook.us6.list-manage.com/subscribe/post?u=a552ad4e61&amp;id=b9e77bb313" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank">
                        <b-form-group
                            label="Email Address"
                            label-for="mce-EMAIL">
                            <b-input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL" required/>
                        </b-form-group>
                        <b-form-group
                            label="First Name"
                            label-for="mce-FNAME">
                            <b-input type="text" value="" name="FNAME" class="" id="mce-FNAME"/>
                        </b-form-group>
                        <b-form-group
                            label="Last Name"
                            label-for="mce-LNAME">
                            <b-input type="text" value="" name="LNAME" class="" id="mce-LNAME" />
                        </b-form-group>
                        <div id="mce-responses" class="clear">
                            <div class="response" id="mce-error-response" style="display:none"></div>
                            <div class="response" id="mce-success-response" style="display:none"></div>
                        </div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
                        <div style="position: absolute; left: -5000px;" aria-hidden="true">
                            <input type="text" name="b_a552ad4e61_b9e77bb313" tabindex="-1" value="">
                        </div>
                        <b-form-group>
                            <b-button
                                type="submit"
                                value="Subscribe"
                                name="subscribe"
                                id="mc-embedded-subscribe"
                                variant="success">
                                Subscribe
                            </b-button>
                        </b-form-group>
                    </form>
                </div>

                <!--End mc_embed_signup-->
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
    export default {
        name: 'Contact',
        data () {
            return {
                title: 'Contact Us',
            }
        }
    }
</script>

<style lang="scss">
    #contact {
        background: #BF1932;
        padding: 40px;

        h2, p, address {
            color: #fff;
        }

        h3 {
            color: #F4CC24;
        }

        a {
            font-weight: bold;
            font-size: 21px;
            color: #fff;
            letter-spacing: -0.53px;
            text-decoration: none;

            &.phone {
                font-size: 15px;
                font-weight: normal;
            }
        }

        a:hover {
            text-decoration: underline;
        }

        label {
            color: #fff;
        }
    }
</style>