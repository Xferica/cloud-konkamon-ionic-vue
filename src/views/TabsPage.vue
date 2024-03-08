<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom" color="primary">
        <ion-tab-button tab="home" href="/tabs/home">
          <ion-icon aria-hidden="true" :icon="home" />
          <ion-label>Home</ion-label>
        </ion-tab-button>
        <ion-tab-button tab="member" href="/tabs/member">
          <ion-icon aria-hidden="true" :icon="people" />
          <ion-label>Member</ion-label>
        </ion-tab-button>
        <ion-tab-button tab="project" href="/tabs/project">
          <ion-icon aria-hidden="true" :icon="document" />
          <ion-label>Project</ion-label>
        </ion-tab-button>
        <ion-tab-button tab="v.modal" id="present-alert">
          <ion-icon aria-hidden="true" :icon="chatbox"/>
          <ion-label>V.Modal</ion-label>
        </ion-tab-button>
        <ion-tab-button tab="Otro más" @click="cambiatexto">
          <ion-icon :icon="camera" />
          <ion-label>{{ texto }}</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
  <ion-alert
    trigger="present-alert"
    header="Project"
    message="Un mensaje cualquiera de aviso"
    :buttons="['OK']"
  ></ion-alert>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import {
  IonTabBar,
  IonAlert,
  IonTabButton,
  IonTabs,
  IonLabel,
  IonIcon,
  IonPage,
  IonRouterOutlet,
  IonicVue,
} from "@ionic/vue";
import { document, home, people, chatbox, camera } from "ionicons/icons";

const texto = ref("bot"); 
function cambiatexto() {
  texto.value = "Mi Botón";
}

</script>
