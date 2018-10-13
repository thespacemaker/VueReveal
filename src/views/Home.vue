<template>
  <v-container fluid>
    <v-layout row wrap>
      <v-flex xs12 sm6 pa-4>
        <v-card>
          <iframe class="resp-iframe" src="presentations/pythonbasics.html"></iframe>
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Python Basics</h3>
              <div>An introductory course to Python syntax</div>
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange" href="presentations/pythonbasics.html">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>

      <v-flex xs12 sm6 pa-4>
        <v-card>
          <iframe class="resp-iframe" src="presentations/fusionbasics.html"></iframe>
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Fusion 360</h3>
              <div>Introduction to Fusion 360</div>
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange" href="presentations/fusionbasics.html">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>

      <v-flex xs12 sm6 pa-4>
        <v-card>
          <object type="text/html" data="presentations/pythonbasics.html">
          </object>
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Coming Soon...</h3>
              <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange" href="presentations/pythonbasics.html">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>

      <v-flex xs12 sm6 pa-4>
        <v-card>
          <iframe class="resp-iframe" src="presentations/pythonbasics.html"></iframe>
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Coming Soon...</h3>
              <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange" href="presentations/pythonbasics.html">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      cards: [
        { title: 'Pre-fab homes', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 12 },
        { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 6 },
        { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 6 }
      ]
    })
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.resp-iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    border: 0;
}
</style>
