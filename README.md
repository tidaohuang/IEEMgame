# IEEMgame
2017工工營課程股產銷遊戲
{Teamleader}

<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <title>Vuetify Components Test</title>
    <link href='https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons' rel="stylesheet" type="text/css">
    <link href="https://unpkg.com/vuetify/dist/vuetify.min.css" rel="stylesheet" type="text/css">
    <!--Add-->
    <link href="http://fonts.googleapis.com/earlyaccess/notosanstc.css" rel="stylesheet" type="text/css">
    <!--Add End-->
    <script src="https://unpkg.com/vue/dist/vue.js"></script>
    <script src="https://unpkg.com/vuetify/dist/vuetify.min.js"></script>
    <title>
        Teamleader
    </title>
</head>

<body>
    <div id="app">
                        <!-- You can add some components here to test. -->
        
    <!--MY CSS-->
    <style>
        #pic_center {
            display:block; 
            margin:auto;   
            width:50%;         
        }
        #div_center1{ 
            width:100%;
            height:10%;
            text-align:center;
            /*;border:1px #000000 dashed;*/
        }
        #div_center2{ 
            width:100%;
            height:50%;
            text-align:center;
            /*;border:1px #000000 dashed;*/
        }
         #div_amount{ 
            width:10%;
            text-align:center;
            background-color:#ff458e;
            /*;border:1px #000000 dashed;*/
        }
      h1 h2 h3{
          font-family: Microsoft JhengHei
       }
        p{
            font-size:1.17em;
        }
        #white{
            background-color:#ffffff;
        }
        
        @import url(//fonts.googleapis.com/earlyaccess/notosanstc.css);  /*思源黑體*/

    </style>    <!--MY CSS END-->
       
    <div>
        <div id="div_center1" style="background-color:#34bdeb;">
            <h1 style="text-align:left">Teamleader<font size="7" style="font-family:Microsoft JhengHei">&nbsp;成本結算</font></h1>
            <h2 style="text-align:right">Day/Time/Money</h2>
        </div>
        <div id="div_center1" style="background-color:#ffffff;">
             <!--some images-->
        </div>  
          <!--TABS-->
        <div>
            <v-tabs id="mobile-tabs-4" grow icons>
                <v-tab-item href="#mobile-tabs-4-1" slot="activators">
                    <h4 style="font-family: Microsoft JhengHei">Retailer</h4>
                </v-tab-item>
                <v-tab-item href="#mobile-tabs-4-2" slot="activators">
                    <h4 style="font-family: Microsoft JhengHei">Wholesaler</h4>
                </v-tab-item>
                <v-tab-item href="#mobile-tabs-4-3" slot="activators">
                    <h4 style="font-family: Microsoft JhengHei">Manufacturer</h4>
                </v-tab-item>
                <v-tab-content v-for="i in 3" key="i"
                               v-bind:id="'mobile-tabs-4-' + i"
                               slot="content">
                    <v-card>
                        <v-card-text>
                            <!--插入切換的內容-->
                            <v-card-text>
                                <div class="text-xs-center">
                                    <v-modal v-model="model">
                                        <v-btn slot="activator" primary dark>倉庫</v-btn>
                                        <v-card id="white">
                                            <v-card-text>
                                            <!--<v-card-text class="subheading grey--text">-->
                                                <!--INPUT-->
                                                <v-card class="grey lighten-4 elevation-0">
                                                    <v-card-text>
                                                        <v-container fluid>
                                                            <v-row row>
                                                                <v-col xs8>
                                                                    <v-text-field name="input-1" label="數量"></v-text-field>
                                                                </v-col>
                                                            </v-row>
                                                        </v-container>
                                                    </v-card-text>
                                                </v-card>
                                                <!--INPUT END-->
                                            </v-card-text>
                                            <v-card-row actions>
                                                <v-spacer></v-spacer>
                                                <v-btn flat v-on:click.native="modal = false" class="primary--text"><font color="#000000">Cancel</font></v-btn>
                                                <v-btn flat v-on:click.native="modal = false" class="primary--text"><font color="#000000">Submit</font></v-btn>
                                            </v-card-row>
                                        </v-card>
                                    </v-modal>
                                </div>
                            </v-card-text>

                            <v-card-text>
                                <div class="text-xs-center">
                                    <v-modal v-model="model">
                                        <v-btn slot="activator" primary dark>物流</v-btn>
                                        <v-card id="white">
                                            <v-card-text>
                                                <!--<v-card-text class="subheading grey--text">-->
                                                <!--INPUT-->
                                                <v-card class="grey lighten-4 elevation-0">
                                                    <v-card-text>
                                                        <v-container fluid>
                                                            <v-row row>
                                                                <v-col xs8>
                                                                    <v-text-field name="input-1" label="數量"></v-text-field>
                                                                </v-col>
                                                            </v-row>
                                                        </v-container>
                                                    </v-card-text>
                                                </v-card>
                                                <!--INPUT END-->
                                            </v-card-text>
                                            <v-card-row actions>
                                                <v-spacer></v-spacer>
                                                <v-btn flat v-on:click.native="modal = false" class="primary--text"><font color="#000000">Cancel</font></v-btn>
                                                <v-btn flat v-on:click.native="modal = false" class="primary--text"><font color="#000000">Submit</font></v-btn>
                                            </v-card-row>
                                        </v-card>
                                    </v-modal>
                                </div>
                            </v-card-text>
                            <!--切換的內容 END-->
                        </v-card-text>
                    </v-card>
                </v-tab-content>
            </v-tabs>

         </div>
            <!--TABS END-->
    </div>
</div>
    <script type="text/javascript">
    let app = new Vue({
      el: '#app',
      data: {
        // add some property here
      }
    })
    </script>
</body>
</html>

