<template>
    <div class = "container-content-alert" v-if="opencontent" @didDismiss="closecontent(false)">
        <ion-input placeholder="masukan header" label="Header" v-model="header"></ion-input>
        <ion-input placeholder="masukan sub header" label="Sub Header" v-model="subheader"></ion-input>
        <ion-input placeholder="masukan pesan" label="Pesan" v-model="content"></ion-input>
    <ion-button class="button-form" @click="presentAlert">
        Xerrr
    </ion-button>
    </div>
</template>
<script setup>
import {ref, defineModel, computed} from "vue";
import data from "../../data/data.json";
import { alertController } from '@ionic/vue';

const storage = ref(data.datakirim)

const header = ref('')
const subheader = ref('')
const content = ref('')

console.log(storage.value)
const openModal = ref(false)

const openModalHandler = () => {
    openModal.value = true 
}

const opencontent = defineModel({
    type: Boolean,
    default: false,
    required: true
})

const presentAlert = async () => {
    const alert = await alertController.create({
    header: 'are you azhar?',
    subheader: 'if yes click action',
    message: 'good, youre very smart son azhar',
    buttons: ['Action'],
    });

    await alert.present();
};

</script>
<style>
</style> 