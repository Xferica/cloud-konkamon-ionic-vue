<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color="primary" mode="ios">
        <ion-title>Título de portada</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-grid :fixed="true">
        <ion-row class="ion-justify-content-center">
          <ion-col size="12" size-lg="4">
            <ion-card>
              <img alt="Silhouette of mountains" src="../../public/scitechBuilding.jpg" />
              <ion-card-header>
                <ion-card-title>título de la tarjeta</ion-card-title>
                <ion-card-subtitle>subtítulo de la tarjeta</ion-card-subtitle>
              </ion-card-header>

              <ion-card-content>
                <p>Este es un párrafo normal dentro del contenido de la tarjeta</p>
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
