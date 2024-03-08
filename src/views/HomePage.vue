<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color="primary" mode="ios">
        <ion-title>Título de la web</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-grid :fixed="true">
        <ion-row class="ion-justify-content-center">
          <ion-col size="12" size-lg="4">
            <ion-card>
              <img alt="Silhouette of mountains" src="/me-rmutsv-square.jpg" />
              <ion-card-header>
                <ion-card-title>Título de la tarjeta</ion-card-title>
                <ion-card-subtitle>subtítulo</ion-card-subtitle>
              </ion-card-header>

              <ion-card-content>
                <p>Este es un texto normal de un párrafo dentro del contenido de la tarjeta.</p>
              </ion-card-content>
            </ion-card>
          </ion-col>
        </ion-row>
      </ion-grid>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
  IonCard,
  IonCardHeader,
  IonCardContent,
  IonCardTitle,
  IonCardSubtitle,
  IonGrid,
  IonRow,
  IonCol,
} from "@ionic/vue";
</script>
