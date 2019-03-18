<template>
    <b-container fluid id="ceremonies">
        <b-row>
            <b-col>
                <h2>{{title}}</h2>
                <p><b>Dana (Offering)</b><br>
                Dana is generosity or giving, a form of alms. It is the practice of cultivating generosity, characterized by unattached and unconditional generosity, giving and letting go. Dana as a formal religious act has the effect of purifying and transforming the mind of the benefactor. Giving without seeking anything in return is foundational spiritual practice. While many of our programs are free, Dae Yen Sa subsists largely on the donations of members and guests. We thank you in advance for your generosity.</p>

                <p><b>Days of Refuge (Retreats)</b><br>
                Dae Yen Sa offers a full Day of Refuge each first Saturday of the month for Seon meditation practice. In addition, we are available to lead groups who may be interested in scheduling their own day of meditation and mindfulness. Dae Yen Sa has welcomed many groups; from spiritual organizations, high schools, colleges, womens’ groups, to religious, interfaith and cultural groups. </p>

                <p><b>Attire</b><br>
                Please dress comfortably and respectfully. Loose fitting pants, yoga or sweat pants allow the most comfortable range of movement when practicing sitting meditation, yoga and qi gong. Please wear appropriate shirts and tops, avoiding provocative styles and inappropriate graphics. Shoes must be removed upon entering the temple.</p>

                <p><b>The Grounds</b><br>
                Dae Yen Sa temple is located in rural New Hartford, CT. As such, we are surrounded by nature—crushed stone and dirt paths, grassy slopes, sometimes mud, snow, ice, etc. We do our best to keep walkways clean and clear, and ask guests to move around the property mindfully and carefully. We have several devotional sites on the property where individuals may make offerings, and practice walking meditation. Grounds are not wheelchair accessible at this time.</p>

                <hr>

                <p><b>Buddha Birthday & Lotus Lantern Celebration – 부처님 오신날:</b><br>
                Yearly celebration includes lotus lantern offerings, traditional liturgy, bathing baby Buddha ceremony, and community reception with vegetarian meal (May).</p>

                <p><b>Baek Jung Cheondo Jae Annual Memorial Service:</b><br>
                Collective yearly service for Deceased Ancestors (August).<br>
                For more information please <a href="mailto:daeyensatemple@gmail.com">contact us</a>.</p>

                <p><b>Cheondo Jae Memorial Services:</b><br>
                By Request service for Deceased Ancestors.<br>
                For more information please <a href="mailto:daeyensatemple@gmail.com">contact us</a>.</p>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
  name: 'Ceremonies',
  data () {
    return {
        title: 'Ceremonies',
    }
  }
}
</script>

<style lang="scss">
    #ceremonies {
        background: #FFB400;
        padding: 40px;

        hr {
            border-top: 0 none;
            border-bottom: 1px solid #EA4B23;
            margin: 40px 0;
        }
    }
</style>