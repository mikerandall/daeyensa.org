<template>
    <b-container fluid id="schedule">
        <b-row>
            <b-col sm="12" md="6">
                <h2>{{title}}</h2>
                <p>Individuals and groups are invited for seon meditation, practice and study. In addition to the regular schedule below, celebrations and ceremonies are held throughout the year. To receive regular information/announcements about events and programs please contact us with your request.</p>
                <h3>All are welcome!</h3>
            </b-col>
            <b-col sm="12" md="6">
                <h4>{{todaysFullDate}}</h4>
                <p v-if="days[this.today] === 'Wednesday'">
                    <b>Daily Morning Kido</b><br>
                    Chanting/Bowing Practice<br>
                    5:15 am — 6:50 am<br>
                    Cheon Su Kyeong/Jebul Tong Cheong/<br>
                    Shin Jung Cheong & Bowing/Gwan Eum Cheong<br>
                    <br>
                    <b>Morning Seon Meditation (Monday-Friday)</b><br>
                    7:00 am — 7:30 am<br>
                    <br>
                    <b>Wednesday Evening Practice</b><br>
                    7:00 pm — 8:30 pm<br>
                    Opening Temple Ceremony<br>
                    Ringing the bell<br>
                    Meditation<br>
                    Chanting or Walking Meditation<br>
                    Fruit and tea party!<br>
                    Temple closes at 8:30 pm.
                </p>
                <p v-if="days[this.today] === 'Saturday'">
                    <b>Daily Morning Kido</b><br>
                    Chanting/Bowing Practice<br>
                    5:15 am — 6:50 am<br>
                    Cheon Su Kyeong/Jebul Tong Cheong/<br>
                    Shin Jung Cheong & Bowing/Gwan Eum Cheong<br>
                    <br>
                    <b>Morning Seon Meditation (Monday-Friday)</b><br>
                    7:00 am — 7:30 am<br>
                    <br>
                    <b>Saturday Morning Practice</b><br>
                    9:00 am — 1:00 pm <br>
                    Body work (either Qigong or Yoga)<br>
                    Short dharma talk<br>
                    Tea prayer<br>
                    Ringing the bell<br>
                    Meditation<br>
                    Chanting<br>
                    Dharma Talk<br>
                    Meditation, sharing, or more chanting<br>
                    Vegetarian lunch served from 12:00 pm — 1:00 pm.
                </p>
                <p v-if="['Wednesday', 'Saturday'].includes(days[this.today]) === false">
                    <b>Daily Morning Kido</b><br>
                    Chanting/Bowing Practice<br>
                    5:15 am — 6:50 am<br>
                    Cheon Su Kyeong/Jebul Tong Cheong/<br>
                    Shin Jung Cheong & Bowing/Gwan Eum Cheong<br>
                    <br>
                    <b>Morning Seon Meditation (Monday-Friday)</b><br>
                    7:00 am — 7:30 am<br>
                </p>

                <p>
                    <b-button class="day-previous btn btn-lg" @click="prevDay">
                        Prev
                        <svg id="i-backwards" viewBox="0 0 32 32" width="32" height="32" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="9.375%">
                            <path d="M16 2 L2 16 16 30 16 16 30 30 30 2 16 16 Z" />
                        </svg>
                    </b-button>

                    <b-button class="day-next btn btn-lg" @click="nextDay">
                        Next
                        <svg id="i-forwards" viewBox="0 0 32 32" width="32" height="32" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="9.375%">
                            <path d="M16 2 L30 16 16 30 16 16 2 30 2 2 16 16 Z" />
                        </svg>
                    </b-button>
                </p>
            </b-col>
        </b-row>

    </b-container>
</template>

<script>
    let date = new Date();
    const days = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'],
        months = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December'];
    export default {
        name: 'Schedule',
        data () {
            return {
                title: 'Temple Schedule',
                date,
                days,
                months,
                today: date.getDay(),
                todaysFullDate: `${days[date.getDay()]}, ${months[date.getMonth()]} ${date.getDate()}`,
                nextDay: () => {
                    let result = new Date(date);
                    result.setDate(result.getDate() + 1);
                    date = result;
                    this.today = date.getDay();
                    this.todaysFullDate = `${days[date.getDay()]}, ${months[date.getMonth()]} ${date.getDate()}`;
                    return date;
                },
                prevDay: () => {
                    let result = new Date(date);
                    result.setDate(result.getDate() - 1);
                    date = result;
                    this.today = date.getDay();
                    this.todaysFullDate = `${days[date.getDay()]}, ${months[date.getMonth()]} ${date.getDate()}`;

                    return date;
                }
            }
        }
    }
</script>

<style lang="scss">

    #schedule {
        background: #F4CC24;
        background-image: url(./assets/Lotus.png);
        background-position: bottom left;
        background-repeat: no-repeat;
        padding: 40px;

        .daily {
            font-family: NotoSans;
            font-size: 20px;
            color: #000000;
        }

        button.day-next {
            float: right;
        }

        button.day-previous {
            float: left;
        }
    }

</style>