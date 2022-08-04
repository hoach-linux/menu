<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-menu-button color="primary"></ion-menu-button>
        </ion-buttons>
        <ion-title>{{ $route.params.id }}</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">{{ $route.params.id }}</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-list>
        <ion-list-header> Recent Conversations </ion-list-header>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-finn.png" />
          </ion-avatar>
          <ion-label>
            <h2>Finn</h2>
            <h3>I'm a big deal</h3>
            <p>Listen, I've had a pretty messed up day...</p>
          </ion-label>
        </ion-item>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-han.png" />
          </ion-avatar>
          <ion-label>
            <h2>Han</h2>
            <h3>Look, kid...</h3>
            <p>I've got enough on my plate as it is, and I...</p>
          </ion-label>
        </ion-item>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-rey.png" />
          </ion-avatar>
          <ion-label>
            <h2>Rey</h2>
            <h3>I can handle myself</h3>
            <p>You will remove these restraints and leave...</p>
          </ion-label>
        </ion-item>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-luke.png" />
          </ion-avatar>
          <ion-label>
            <h2>Luke</h2>
            <h3>Your thoughts betray you</h3>
            <p>I feel the good in you, the conflict...</p>
          </ion-label>
        </ion-item>
      </ion-list>

      <ion-list fullscreen>
        <ion-list-header> Online </ion-list-header>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-poe.png" />
          </ion-avatar>
          <ion-label>
            <h2>Poe</h2>
            <h3>New Ride</h3>
            <p>I just upgraded my X-Wing. Next time...</p>
          </ion-label>
        </ion-item>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-ben.png" />
          </ion-avatar>
          <ion-label>
            <h2>Ben</h2>
            <h3>Move Along</h3>
            <p>These aren't the droids you're looking for...</p>
          </ion-label>
        </ion-item>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-leia.png" />
          </ion-avatar>
          <ion-label>
            <h2>Leia</h2>
            <h3>You're My Only Hope</h3>
            <p>I've placed information vital to the survival...</p>
          </ion-label>
        </ion-item>

        <ion-item>
          <ion-avatar slot="start">
            <img src="@/img/avatar-yoda.png" />
          </ion-avatar>
          <ion-label>
            <h2>Yoda</h2>
            <h3>Size matters not</h3>
            <p>Do or do not. There is no try...</p>
          </ion-label>
        </ion-item>
      </ion-list>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonItem, IonList, IonLabel } from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: {
    IonItem,
    IonList,
    IonLabel,
  },
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
