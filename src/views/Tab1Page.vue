<template>
  <ion-page>
    <ion-header>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>
      <div class="gambar">
    <IconAccessibleFilled size="150px"/>
  </div>
      <div class="container">
      <ion-button id="xer">
        xerr
      </ion-button>
      <!-- <KepalaView name="Xeryux" /> -->
    </div>
    <ion-alert
  trigger="xer"
  header="Alex The Best"
  subHeader="father dhafin"
  message="because father dhafin is the super hero"
  :buttons="alertButtons"
></ion-alert>
    </ion-content>
  </ion-page>
</template>

<script setup lang="js">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, } from '@ionic/vue';
import { IconAccessibleFilled } from '@tabler/icons-vue';
// import KepalaView from '@/components/KepalaView.vue';
</script>
