<template>
  <div id="app">
    <Flicking :options="{ align: 'prev', circular: true }">
      <div class="panel">
        <div class="image-data" style="background-image:url('https://i.pinimg.com/originals/ef/7f/b1/ef7fb1b37078b6a2aef8e40710446bfa.jpg')"></div>
      </div>
      <div class="panel">
        <div class="image-data" style="background-image:url('https://wallpapercave.com/wp/wp2719096.jpg')"></div>
      </div>
      <div class="panel">
        <div class="image-data" style="background-image:url('https://i.pinimg.com/736x/7d/98/84/7d98840fdff1b2e7cd508cc7f3a17403.jpg')"></div>
      </div>
    </Flicking>
  </div>
</template>

<script>
import { Flicking } from "@egjs/vue-flicking"
export default {
  name: 'App',
  components: {
    Flicking: Flicking
  }
}
</script>

<style>
  @import url("../node_modules/@egjs/vue-flicking/dist/flicking.css");
  .panel {
    width: 100%;
    height: 500px;
  }

  .image-data {
    width: 100%;
    height: 100%;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    background-color: #dedede;
  }
</style>
