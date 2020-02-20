<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-center">
        <logo />
        <vuetify-logo />
      </div>
      <v-card>
        <v-card-title class="headline">
          会津大学　坂道サークル
        </v-card-title>
        <v-card-text>
          <p>会津大学坂道サークルは2017年７月に出来た　乃木坂４６　欅坂46　日向坂４６好きのためのサークルです。</p>
          <p> The Aizu University Sakamichi Circle is a circle for those who like Nogizaka 46, Keyakizaka 46, and Hyugazaka 46, which were created in July 2017.</p>
          
          <p>坂道サークルの主な活動内容はこちらから! Click here for the main activities of the slope circle!
          <a 
          href="/test"
          > 
          activate
          </a>.
          </p>
          
          <p>今月の予定はこちらから。
            Click here for this month's schedule. <a
              href="https://calendar.google.com/calendar/b/2?cid=YWl6dTQ2c2FrYW1pY2hpQGdtYWlsLmNvbQ"
              target="_blank"
            >
              Calender
            </a>.
          </p>
          <p>乃木坂４６　欅坂４６　日向坂４６の情報はこちら。
            Click here for sakamichi imformation. <a
           href="/test"
            >
              Sakamichi imformation 
             
            </a>.
          </p>
          <p>公式ツイッターはこちらから
            Click here for oficial Twitter <a
              href="https://twitter.com/aizu_sakamithi"
              target="_blank"
              title="contribute"
            >
              Twitter
            </a>.
          </p>
          <p>興味がある方、合同飲み会希望の方はTwitterもしくはGmailでご連絡ください</p>
          <div class="text-xs-right">
            <em><small>&mdash; 会津大学坂道サークル</small></em>
          </div>
          <hr class="my-3">
          <a
            href="https://nuxtjs.org/"
            target="_blank"
          >
            Nuxt Documentation
          </a>
          <br>
          <a
            href="https://github.com/nuxt/nuxt.js"
            target="_blank"
          >
            Nuxt GitHub
          </a>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>
