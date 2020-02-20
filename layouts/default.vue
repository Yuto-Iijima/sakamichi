<template>
  <v-app>
   

    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
    >
    
      
   
      
      <v-btn to="/" class="ma-md-4">
      <v-toolbar-title v-text="title" />
      </v-btn>

      <v-btn
      class="ma-md-4"
       @click.stop="clipped = !clipped"
        href="/active">
      Activate
      </v-btn>
      <v-btn
      class="ma-md-4"
       @click.stop="clipped = !clipped"
        href="https://calendar.google.com/calendar/b/2?cid=YWl6dTQ2c2FrYW1pY2hpQGdtYWlsLmNvbQ"
        target="_blank">
      Calender
      </v-btn>
      <v-btn
      class="ma-md-4"
       @click.stop="clipped = !clipped"
        href="/test">
      Information
      </v-btn>
      <v-spacer />
    
    </v-app-bar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
    
    
    <v-footer
      :fixed="fixed"
      app
    >
      <span>{{year}}/</span><span>{{month}}/</span><span>{{date}}</span>
    </v-footer>

  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Activate',
          to: '/active'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'saka imformation',
          to: '/test'
        }
      ],

      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: '会津大学坂道サークル',
      year: new Date().getFullYear(),
      month: new Date().getMonth() + 1,
      date: new Date().getDate()
    }
  }
}
</script>
