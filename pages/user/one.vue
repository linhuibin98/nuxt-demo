<template>
  <div class="main">UserOne</div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component({})
export default class UserOne extends Vue {}
</script>

<style lang="scss">
.main {
  background-color: #ff0f;
  text-align: center;
}
</style>
