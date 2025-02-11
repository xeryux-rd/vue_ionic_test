<template>
    <ion-header>
        <ion-toolbar>
            <ion-title>
                {{title}}
                <p>Explore <a target="_blank" rel="noopener noreferrer" href="https://ionicframework.com/docs/components">UI Components</a></p>
            </ion-title>
        </ion-toolbar>
    </ion-header>
</template>
<script setup>
defineProps({
    title:String,
})
</script>