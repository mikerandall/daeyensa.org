<template>
    <b-container fluid id="footer">
        <b-row>
            <b-col>
                <p>Copyright © 2019 Dae Yen Sa International Temple and Meditation Center</p>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
  name: 'Foot',
  data () {
    return {
        title: 'Footer',
    }
  }
}

</script>

<style lang="scss">
    #footer {
        background: #E76B27;
        color: #FFFFFF;
        text-align: center;

        .row {
            margin-right: 0;
            margin-left: 0;
        }

        p {
            height: 200px;
            vertical-align: middle;
            display: flex;
            flex-direction: column;
            justify-content: center;

        }
    }
</style>