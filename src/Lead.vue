<template>
    <div id="lead">
        <div class="logo">
            <img src="./assets/LogoWhite.png" fluid border="0">
            <p>댸연불보정사<br>
            케네티컷 ~ 성역 관음성지<br>
            19 Kinsey Road,<br>
            New Hartford, CT 06057<br>
            860-489-3254</p>
        </div>
        <b-carousel id="carousel1"
                    style="text-shadow: 1px 1px 2px #333;"
                    indicators
                    background="#ababab"
                    :interval="0"
                    img-width="1024"
                    img-height="480"
                    v-model="slide"
                    @sliding-start="onSlideStart"
                    @sliding-end="onSlideEnd">
            <b-carousel-slide>
                <img
                    slot="img"
                    class="d-block img-fluid w-100"
                        src="./assets/banya_at_unity-sm.jpg" srcset="./assets/banya_at_unity-sm.jpg 800w, ./assets/Banya_at_unity.jpg 810w"
                    alt="Banya Sunim gives Dharma talk at Unity in the Foothills."
                />
                <p>
                    Ban Ya Sunim (AKA Reverand Brian) spoke at <a href="http://www.unityinthefoothillsct.org" target="_blank">Unity in the Foothills</a> in February. You can listen to that dharma talk below!<br/>
                    <audio src="http://www.unityinthefoothillsct.org/sites/unityinthefoothillsct.org/files/2019_02-17RevBrianLessonMeditation.mp3" controls="" controlslist="nodownload"></audio>
                </p>
            </b-carousel-slide>

            <b-carousel-slide>
                <img
                    slot="img"
                    class="d-block img-fluid w-100"
                        src="./assets/DSC_0348-sm.jpg" srcset="./assets/DSC_0348-sm.jpg 800w, ./assets/DSC_0348.jpg 810w"
                    alt="Twin Pagodas on the temple grounds."
                />
                <p>For over 30 years Dae Yen Sa has been a place of refuge for those seeking liberation from the bonds of greed, hatred and ignorance. Rooted in the ground of Korean Seon (Zen) Buddhism, and under the direction of Abbot, Ven. Dae San Dae Sa, we offer instruction and practice in seon meditation, chanting, and dharma study, as well as Yoga and Qigong.</p>
            </b-carousel-slide>

            <b-carousel-slide>
                <img
                    slot="img"
                    class="d-block img-fluid w-100"
                        src="./assets/DSC_0404-sm.jpg" srcset="./assets/DSC_0404-sm.jpg 800w, ./assets/DSC_0404.jpg 810w"
                    alt="Monks in ceremony at Dae Yen Sa Temple."
                />
                <p>We hold traditional ceremonies, and conduct retreat days for individuals and groups throughout the year.<br>
        Be Buddha! 성불 핲시다</p>
            </b-carousel-slide>
        </b-carousel>
    </div>
</template>

<script>
export default {
  name: 'Lead',
  data () {
    return {
        slide: 0,
        msg: 'Lead carousel.',
        onSlideStart: ()=>{},
        onSlideEnd: () =>{}
    }
  }
}
</script>

<style lang="scss">
    #lead {
        position: relative;
        .logo {
            position: absolute;
            top: 20px;
            left: 20px;
            z-index: 100;
            width: 70px;

            img {
                width: 70px;
            }

            p {
                display: none;
                font-size: 12px;
                line-height: 15px;
                color: #FFFFFF;
                text-align: center;
                text-shadow: 0 2px 4px rgba(0,0,0,0.65);
            }
        }

        .carousel-caption {
            background-color: rgba(0,0,0,0.65);
            right: 0;
            left: 0;
            bottom: 0;
            padding: 20px;

            p {
                color: #FFFFFF;
                display: block;
                font-size: 16px;
                line-height: 20px;
                text-align: center;
                margin: 15px 15px;
            }

            audio {
                margin: 15px auto;
            }
        }

        @media (min-width: 500px) {
            .logo {
                top: 40px;
                left: 40px;
                width: 100px;

                img {
                    width: 100px;
                }

                p {
                    display: block;
                }

            }
        }

        @media (min-width: 800px) {

            .carousel-caption {
                p {
                    font-size: 19px;
                    line-height: 28px;
                }
            }

            .logo {
                width: 200px;

                img {
                    width: 200px;
                }

                p {
                    font-size: 19px;
                    line-height: 28px;
                }
            }
        }
    }
</style>
