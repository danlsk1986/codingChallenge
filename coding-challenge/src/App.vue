<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>    
    <HeroComponent></HeroComponent>
    <MenuComponent></MenuComponent>
    <ProductComponent></ProductComponent>
  </div>
</template>

<script>

import HeaderComponent from './components/HeaderComponent.vue';
import HeroComponent from './components/HeroComponent.vue';
import MenuComponent from './components/MenuComponent.vue';
import ProductComponent from './components/ProductComponent';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    HeroComponent,
    MenuComponent,
    ProductComponent
    
  }
}
</script>

<style>

@import './assets/css/styles.css';
</style>
