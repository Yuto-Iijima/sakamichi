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
    <v-carousel
     cycle
    height="300"
    hide-delimiter-background
    show-arrows-on-hover
    >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
 
  </v-carousel>
  

      <v-card>
       <v-content class="bg">
        <v-card-title class="headline">
          <strong class="green--text text--lighten-2">会津大学　坂道サークル</strong>
        </v-card-title>
        <v-card-text>
          <p>会津大学坂道サークルは2017年７月に出来た　乃木坂４６　欅坂46　日向坂４６好きのためのサークルです。</p>
          <p> The Aizu University Sakamichi Circle is a circle for those who like Nogizaka 46, Keyakizaka 46, and Hyugazaka 46, which were created in July 2017.</p>
          
          <p>坂道サークルの主な活動内容はこちらから! Click here for the main activities of the slope circle!
          <a 
          href="/active"
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
            Click here for sakamichi information. <a
           href="/test"
            >
              Sakamichi information 
             
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
            <em><small>&mdash;会津大学坂道サークル</small></em>
          </div>
          <hr class="my-3">
          <a
            href="mailto:aizu46sakamichi&#64;gmail.com"
            target="_blank"
          >
            aizu46sakamichi@gmail.com
          </a>
          <br>
           <v-row>
           <v-layout justify-center>
          <div class="tweet"><a class="twitter-timeline" href="https://twitter.com/aizu_sakamithi?s=09" data-widget-id="699562346964918273" lang="ja" data-chrome="nofooter" height="392"></a>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script></div>
          </div>
          <a href="https://lin.ee/ah58gym"><img height="36" border="0" src="https://scdn.line-apps.com/n/line_add_friends/btn/ja.png"></a>
          </v-layout>
          </v-row>

        </div>
        
        </v-card-text>
        <v-card-actions>
          <v-spacer />
       
        </v-card-actions>
         </v-content>
      </v-card>
    </v-flex>
  </v-layout>
 </v-content>
</template>

<style>
    .bg {
        background-size: cover;
        background-image: url("~@/assets/images/back_sakamichi.png");
    }
</style>

<script>
import img1 from '~/assets/images/花見.jpg'
import img2 from '~/assets/images/花見集合.jpg'
import img3 from '~/assets/images/ライブ１.jpeg'
import img4 from '~/assets/images/アンビ.jpg'
import img5 from '~/assets/images/握手会.jpg'
import img6 from '~/assets/images/QR_saka.png'

export default {
    data () {
      return {
        items: [
          {
            src:img1,frex:12
          },
           {
            src:img2,
            height:300,
            width:300,
          },
           {
            src:img3,frex:12
          },
           {
            src:img4,frex:12
          },
           {
            src:img5,frex:12
          },
        ],
        QR_img:{src:img6},
      }
    },
  }
  
 
</script>
