<template>
<ion-page>
    <ion-tabs>
        <ion-router-outlet></ion-router-outlet>
            <ion-tab-bar slot="botton">
                <ion-tab-button tab="home" href="/home">
                    <ion-icon :icon="playCircle" />
                    <ion-label>home</ion-label>
                </ion-tab-button>
                <ion-tab-button tab="library" href="/library">
                    <ion-icon :icon="library" />
                    <ion-label>Library</ion-label>
                </ion-tab-button>
                <ion-tab-button tab="search" href="/search">
                    <ion-icon :icon="search" />
                    <ion-label>Search</ion-label>
                </ion-tab-button>
                <ion-tab-button tab="radio" href="/radio">
                    <ion-icon :icon="radio" />
                    <ion-label>Radio</ion-label>
                </ion-tab-button>
            </ion-tab-bar>
    </ion-tabs>
</ion-page>
</template>

<script lang="ts" setup>
   import { IonPage, IonTabs, IonTabButton, IonTabBar, IonIcon, IonLabel, IonRouterOutlet } from "@ionic/vue";
   import { playCircle, radio, library, search } from "ionicons/icons";
</script>

<style scoped>

</style>