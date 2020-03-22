<template>
  <v-container fluid>
    <v-layout justify-center align-center>
      <v-flex>
        <v-row justify="center">
          <v-col cols="10">
            <v-card class="elevation-8" v-if="vista == 1">
              <v-toolbar color="primary" dark>
                <v-toolbar-tittle>
                  Login
                </v-toolbar-tittle>
              </v-toolbar>
              <v-card-text>
                <v-text-field label="Email"></v-text-field>
                <v-text-field label="Password" type="password"></v-text-field>
                <div class="my-2">
                  <v-btn @click="vista++" depressed small color="primary" class="elevation-3"
                    >Login</v-btn
                  >
                </div>
              </v-card-text>
            </v-card>
          </v-col>
           <v-col cols="10">
            <v-card class="elevation-8" v-if="vista == 2">
              <v-toolbar color="primary" dark>
                <v-toolbar-tittle>
                  Que te gustaria que agregaramos al informe?
                </v-toolbar-tittle>
              </v-toolbar>
              <v-card-text>
                <v-textarea
                  outlined
                  name="input-7-4"
                  label="Outlined textarea"
                  value="que mejoras le harías al informe"
                ></v-textarea>
                <div class="my-2">
                  <v-btn  @click="vista++" depressed small color="primary" class="elevation-3"
                    >Enviar Respuesta</v-btn
                  >
                </div>
              </v-card-text>
            </v-card>
          </v-col>

          <v-col cols="10">
            <v-card class="elevation-8" v-if="vista == 3">
              <v-toolbar color="primary" dark>
                <v-toolbar-tittle>
                  la informacion es correcta
                </v-toolbar-tittle>
              </v-toolbar>
              <v-card-text>
                <v-radio-group v-model="row" row>
                  <v-radio label="si" value="radio-1"></v-radio>
                  <v-radio label="no" value="radio-2"></v-radio>
                  <v-radio label="mas o menos" value="radio-2"></v-radio>
                </v-radio-group>

                <div class="my-2">
                  <v-btn @click="vista++"  depressed small color="primary" class="elevation-3"
                    >Enviar Respuesta</v-btn
                  >
                </div>
              </v-card-text>
            </v-card>
          </v-col>

          <v-col cols="10">
            <v-card class="elevation-8" v-if="vista == 4">
              <v-toolbar color="primary" dark>
                <v-toolbar-tittle>
                  del 1 al 5 es rapido el sitio
                </v-toolbar-tittle>
              </v-toolbar>
              <v-card-text>
                <v-radio-group v-model="row" row>
                  <v-radio label="1" value="unoacinco-1"></v-radio>
                  <v-radio label="2" value="unoacinco-2"></v-radio>
                  <v-radio label="3" value="unoacinco-3"></v-radio>
                  <v-radio label="4" value="unoacinco-4"></v-radio>
                  <v-radio label="5" value="runoacinco-5"></v-radio>
                </v-radio-group>
                <div class="my-2">
                  <v-btn  @click="vista++"  depressed small color="primary" class="elevation-3"
                    >Finalizar</v-btn
                  >
                </div>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="10">
            <v-card class="elevation-8" v-if="vista == 5">
              <v-toolbar color="primary" dark>
                <v-toolbar-tittle>
                  Muchas Gracias por sus respuestas!!!
                </v-toolbar-tittle>
              </v-toolbar>
            </v-card>
          </v-col>
        </v-row>
      </v-flex>
    </v-layout>
  </v-container>
</template>
<script>
export default {
  data: () => ({
    vista: 1
  })
};
</script>
