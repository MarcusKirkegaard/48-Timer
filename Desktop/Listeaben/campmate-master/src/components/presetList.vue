<template>
        <ul class="presets">
            <li class="preset" @click="addPreset1()">Camping</li>
            <li class="preset" @click="addPreset2()">Festival</li>
            <li class="preset" @click="addPreset3()">Travel</li>
        </ul>
</template>

<script>
import bus from '@/main.js'

export default {
    name: 'preset-list',
  data() {
    return {
      camping: [ting1, ting2, ting3, ting4],
    }
  },
  methods: {
    addPreset1() {
      preventDefault()
      bus.$emit('create-camping', this.camping)
      this.camping.push()
    }
  }
}
</script>

<style>

</style>