<template>
<ion-page>
  <ion-header>
    <ion-toolbar>
      <ion-title>Hola mundo</ion-title>
    </ion-toolbar>
  </ion-header>

  <ion-content class="ion-padding">
    <h1>Hola mundo</h1>
  </ion-content>

  <ion-footer>
    <ion-toolbar>
      <ion-tab-bar slot="button">
        <ion-tab-button>footer</ion-tab-button>
      </ion-tab-bar>
    </ion-toolbar>
  </ion-footer>

</ion-page>
</template>

<script lang="ts" setup>
import { IonPage, IonContent, IonFooter, IonToolbar, IonTitle } from "@ionic/vue";
   
</script>

<style scoped>

</style>