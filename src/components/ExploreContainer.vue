<template>
  <div id="container">

     <ion-text>Disable checkbox issue</ion-text>
    <ion-item>
        <ion-label>Apple</ion-label>
       <ion-checkbox slot="start" color="primary" ></ion-checkbox>
       
    </ion-item>

     <ion-item>
       <ion-label>Windows</ion-label>
       <ion-checkbox slot="start"  color="primary" disabled="true" ></ion-checkbox>
       
    </ion-item>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ExploreContainer',
  props: {
    name: String
  }
});
</script>

<style scoped>
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: #8c8c8c;
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
