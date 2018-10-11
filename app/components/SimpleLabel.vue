<template>
    <Page>
        <Label class="title" :text="computedText"  col="1"/>
    </Page>
</template>

<script lang="ts">
import Vue from 'nativescript-vue';
import { Component } from 'vue-property-decorator';

  @Component({})
  export default class Simple extends Vue{
    get computedText() {
      return 'Computed text';
    }
  }
</script>

<style scoped>
    .title {
        text-align: left;
        padding-left: 16;
    }
</style>
