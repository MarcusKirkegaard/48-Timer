<template>
  <div class="home">
    <h1>CAMP MATE</h1>
    <preset />
    <list />
  </div>
</template>

<script>
// @ is an alias to /src
import topbob from '@/components/topbob.vue'
import list from '@/components/list.vue'
import preset from '@/components/preset.vue'
import {
  db
} from '../firebaseConfig'


export default {
  name: 'home',
  components: {
    topbob,
    list,
    preset
  }
}


</script>

<style>
  h1 {
    font-size: 3rem;
    padding: 1rem;
    margin: 0;
    color: #ffffff;
    background-color: black;
  }

  .preset-menu {
    margin: 1% 25%;
    text-align: left;
  }

  .presets {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-gap: 1%;
    text-align: center;
  }

  .preset {
    background-color: red;
    padding: 2%;
    cursor: pointer;
  }

  p img {
      transform: rotate(0deg);
      width: 1.5%;
    }

  p img:hover {
      transform: rotate(90deg);
      width: 1.5%;
    }
</style>
