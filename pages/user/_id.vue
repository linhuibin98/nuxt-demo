<template>
  <div>
    <span>{{ name }}</span>
    <span>{{ $route.params.id }}</span>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component({})
export default class UserIndex extends Vue {
  public name: string = '用户id为：'

  asyncData({ params, redirect }: any): void {
    if (params.id === '99') {
      redirect('/user/one')
    }
  }
}
</script>

<style></style>
