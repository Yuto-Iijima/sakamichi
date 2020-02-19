<template>
  <v-card
    class="mx-auto"
    max-width="500"
  >
    <v-toolbar color="#7D2982">
     <v-toolbar-title>乃木坂46</v-toolbar-title>
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
              <v-spacer></v-spacer>

              <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-bookmark</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-share-variant</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
       </v-row>
    </v-container>
  </v-card>
</template>

<script>
import img from '~/assets/images/nogi1.jpg';
import img2 from '~/assets/images/nogi2.jpeg';
import img3 from '~/assets/images/nogi3.jpg';


  export default {
    data: () => ({
      cards: [
        { title: 'ニュース', src:img, href:"http://www.nogizaka46.com/news/", flex: 12 },
        { title: 'ブログ', src: img2, href:"http://blog.nogizaka46.com/", flex: 6 },
        { title: '動画', src:img3, href:"https://www.youtube.com/channel/UCUzpZpX2wRYOk3J8QTFGxDg", flex: 6 },
      ],
    }),
  }
</script>