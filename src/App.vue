<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Capasitor plugins</ion-title>
      </ion-toolbar>

    </ion-header>
    <ion-content class="ion-padding">

<img :src="imageUrl" alt="">
<button v-on:click="makePhoto">Take Photo</button>

    </ion-content>
  </ion-page>
</template>

<script lang="ts" setup>
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import { Camera, CameraResultType } from '@capacitor/camera';
import { ref } from 'vue';

const imageUrl = ref()

const makePhoto = async () => {
  const image = await Camera.getPhoto({
    quality: 90,
    allowEditing: true,
    resultType: CameraResultType.Uri
  });

  imageUrl.value = image.webPath;
};


</script>
<style scoped>
.full {
  background-color: aqua;
}

.mid {
  background-color: blueviolet;
}

.mid2 {
  background-color: red;
}
</style>