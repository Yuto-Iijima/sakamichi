<template>
  <v-card
    class="mx-auto"
    max-width="350"
  >
    <v-toolbar color="#7CC8E9">
     <v-toolbar-title>日向坂46</v-toolbar-title>
     <v-spacer></v-spacer>
    </v-toolbar>


    <v-container>
      <v-row>
        <v-col
          v-for="card in cards"
          :key="card.title"
          :cols="card.flex"
        >
          <v-card :href="card.href">
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
             
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>

            <v-card-actions>
              
            </v-card-actions>
          </v-card>
        </v-col>
       </v-row>
    </v-container>
  </v-card>
</template>

<script>
import img from '~/assets/images/hinata_news.jpg';
import img2 from '~/assets/images/hinata_blog.jpeg';
import img3 from '~/assets/images/hinata_movie.jpg';


  export default {
    data: () => ({
      cards: [
        { title: 'ニュース', src:img, href:"https://www.hinatazaka46.com/s/official/news/list?ima=0000&dy=202002", flex: 12 },
        { title: 'ブログ', src: img2, href:"https://www.hinatazaka46.com/s/official/diary/member?ima=0000", flex: 6 },
        { title: '動画', src:img3, href:"https://www.hinatazaka46.com/s/official/page/video?ima=0000", flex: 6 },
      ],
    }),
  }
</script>