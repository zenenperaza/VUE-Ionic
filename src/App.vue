<template>

  <ion-page >
    <ion-header>
      <ion-toolbar>
        <ion-title>GRID Example</ion-title>
      </ion-toolbar>
       
    </ion-header>
    <ion-content class="ion-padding"> 
      
      <ion-grid>
        <ion-row>
          <ion-col size="12" class="full">Hello world full with</ion-col>
        </ion-row>
        <ion-row>
          <ion-col size="6" size-xs="12" size-md="12" size-lg="6"  class="mid">50%</ion-col>
          <ion-col size="6"  size-xs="12" size-md="12" size-lg="6" class="mid2">50%</ion-col>
        </ion-row>
      </ion-grid>

    </ion-content>
  </ion-page>
</template>

<script lang="ts" setup>
  import { IonContent, IonHeader, IonMenu, IonMenuButton, IonPage, IonTitle, IonToolbar, IonGrid, IonRow, IonCol } from '@ionic/vue';



</script>
<style scoped>
.full{
  background-color: aqua;
}
.mid {
  background-color: blueviolet;
}
.mid2 {
  background-color: red;
}
</style>