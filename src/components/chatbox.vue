<template>
  <v-sheet
    height="100vh"
    elevation="0"
    color="#F0F0F0"
    tile
  >
    <div class="header">
      <p>Chat</p>
      <div>
        <v-btn icon class="mr-1 d-md-none" @click="dialog = !dialog">
          <v-icon right color="white">mdi-message-outline</v-icon>
        </v-btn>
        <v-btn icon class="mr-1">
          <v-icon right color="white">mdi-account-multiple-outline</v-icon>
        </v-btn>
        <v-btn icon class="mr-1">
          <v-icon right color="white">mdi-filter-outline</v-icon>
        </v-btn>
        <v-btn icon class="mr-1">
          <v-icon right color="white">mdi-magnify</v-icon>
        </v-btn>
      </div>
    </div>
    <div class="vuebar-element" v-bar>
      <v-sheet
        elevation="0"
        color="#fff"
        tile
        class="overflow-y-auto"
      >
        <v-container>
          <v-row>
            <v-col cols="9" offset="3">
              <v-card
                color="#EDEEF8"
                class="sent"
              >
                <v-card-title class="headline grey--text">Lorem ipsum, dolor sit amet.</v-card-title>

                <v-card-subtitle>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiis ad magni, provident eaque laboriosam animi, corrupti eveniet aperiam quod numquam ullam tenetur earum dignissimos sapiente vel. Consequuntur magni iusto inventore!</v-card-subtitle>
                <v-card-actions>
                  <v-list-item class="grow">
                    <v-list-item-avatar color="grey darken-3">
                      <v-img
                        class="elevation-6"
                        src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
                      ></v-img>
                    </v-list-item-avatar>

                    <v-list-item-content>
                      <v-list-item-title  class="d-none d-sm-flex">me</v-list-item-title>
                    </v-list-item-content>

                    <v-row
                      align="center"
                      justify="end"
                      class="d-block d-sm-flex"
                    >
                      <v-btn color="white pink--text">
                        <v-icon left color="pink">mdi-check</v-icon>
                        done
                      </v-btn>
                    </v-row>
                  </v-list-item>
                </v-card-actions>
              </v-card>
              <v-subheader>me<v-spacer></v-spacer>12:20p
                <v-avatar size="36" class="ml-2">
                  <img
                    src="https://cdn.vuetifyjs.com/images/john.jpg"
                    alt="John"
                  >
                </v-avatar>
              </v-subheader>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="9">
              <v-card
                color="#EDEEF8"
                class="recieved"
              >
                <v-card-title class="headline grey--text">Lorem ipsum, dolor sit amet.</v-card-title>

                <v-card-subtitle>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiis ad magni, provident eaque laboriosam animi, corrupti eveniet aperiam quod numquam ullam tenetur earum dignissimos sapiente vel. Consequuntur magni iusto inventore!</v-card-subtitle>
              </v-card>
              <v-subheader>
                <v-avatar size="36" class="mr-2">
                  <img
                    src="https://cdn.vuetifyjs.com/images/john.jpg"
                    alt="John"
                  >
                </v-avatar>
                Sk<v-spacer></v-spacer>
                12:20p
              </v-subheader>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="9" offset="3">
              <v-card
                color="#f0f0f0"
                class="sent"
              >
                <v-card-title class="headline grey--text">Lorem ipsum, dolor sit amet.</v-card-title>

                <v-card-subtitle>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiis ad magni, provident eaque laboriosam animi, corrupti eveniet aperiam quod numquam ullam tenetur earum dignissimos sapiente vel. Consequuntur magni iusto inventore!</v-card-subtitle>
                <v-card-actions>
                  <v-list-item class="grow">
                    <v-list-item-avatar color="grey darken-3">
                      <v-img
                        class="elevation-6"
                        src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
                      ></v-img>
                    </v-list-item-avatar>

                    <v-list-item-content>
                      <v-list-item-title class="d-none d-sm-flex">me</v-list-item-title>
                    </v-list-item-content>

                    <v-row
                      align="center"
                      justify="end"
                      class="d-block d-sm-flex"
                    >
                      <v-btn color="white pink--text">
                        <v-icon left color="pink">mdi-check</v-icon>
                        done
                      </v-btn>
                    </v-row>
                  </v-list-item>
                </v-card-actions>
              </v-card>
              <v-subheader>me<v-spacer></v-spacer>12:20p
                <v-avatar size="36" class="ml-2">
                  <img
                    src="https://cdn.vuetifyjs.com/images/john.jpg"
                    alt="John"
                  >
                </v-avatar>
              </v-subheader>
            </v-col>
          </v-row>
        </v-container>
      </v-sheet>
    </div>
    <v-row class="pa-2 overflow-hidden" no-gutters style="height: 10vh">
      <v-col class="d-none d-md-flex" md="1">
        <v-btn icon x-large>
          <v-icon x-large color="grey-lighten-4">mdi-plus-circle</v-icon>
        </v-btn>
      </v-col>
      <v-col  cols="11" md="10">
        <v-textarea
          rounded
          rows="1"
          background-color="white"
          no-resize placeholder="message"
          color="#222"
          solo
        >
        </v-textarea>
      </v-col>
      <v-col cols="1" md="1" class="pt-1">
        <v-btn icon>
          <v-icon color="blue" right>mdi-send-outline</v-icon>
        </v-btn>
      </v-col>
    </v-row>
    <friends :dialog="dialog"/>
  </v-sheet>
</template>

<script>
import friends from './friends.vue'
export default {
  components: {
    friends
  },
  data () {
    return {
      dialog: false
    }
  }
}
</script>

<style scoped>
 .header {
    height: 7vh;
    font-size: 20px;
    background-color: #48B0B8;
    color: white;
    display: flex;
    justify-content: space-between;
    padding: 10px;
  }
  .sent {
    transform: translateX(-40px);
  }
  .recieved {
    transform: translateX(40px);
  }
  .sent:before {
  content: "";
  width: 0px;
  height: 0px;
  position: absolute;
  border-left: 7px solid #EDEEF8;
  border-right: 7px solid transparent;
  border-top: 7px solid transparent;
  border-bottom: 7px solid #EDEEF8;
  right: -10px;
  bottom: 0px;
}
.recieved:before {
  content: "";
  width: 0px;
  height: 0px;
  position: absolute;
  border-right: 7px solid #EDEEF8;
  border-left: 7px solid transparent;
  border-top: 7px solid transparent;
  border-bottom: 7px solid #EDEEF8;
  left: -10px;
  bottom: 4px;
}
.vuebar-element {
  height: 83vh;
  width: 100%;
  max-width: 100%;
  background: #dfe9fe;
}
.vb > .vb-dragger {
    z-index: 5;
    width: 12px;
    right: 0;
}

.vb > .vb-dragger > .vb-dragger-styler {
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-transform: rotate3d(0,0,0,0);
    transform: rotate3d(0,0,0,0);
    -webkit-transition:
        background-color 100ms ease-out,
        margin 100ms ease-out,
        height 100ms ease-out;
    transition:
        background-color 100ms ease-out,
        margin 100ms ease-out,
        height 100ms ease-out;
    background-color: rgba(48, 121, 244,.1);
    margin: 5px 5px 5px 0;
    border-radius: 20px;
    height: calc(100% - 10px);
    display: block;
}

.vb.vb-scrolling-phantom > .vb-dragger > .vb-dragger-styler {
    background-color: rgba(48, 121, 244,.3);
}

.vb > .vb-dragger:hover > .vb-dragger-styler {
    background-color: rgba(48, 121, 244,.5);
    margin: 0px;
    height: 100%;
}

.vb.vb-dragging > .vb-dragger > .vb-dragger-styler {
    background-color: rgba(48, 121, 244,.5);
    margin: 0px;
    height: 100%;
}

.vb.vb-dragging-phantom > .vb-dragger > .vb-dragger-styler {
    background-color: rgba(48, 121, 244,.5);
}
</style>
