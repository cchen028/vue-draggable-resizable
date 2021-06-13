<template>
  <div id="app">
    <div style="height: 500px; width: 500px; border: 1px solid red; position: relative;">
      <vue-draggable-resizable axis="x" :w="100" :h="50" :y="20" :x="0" :parent="true" :handles="['ml','mr']" :active="true" :prevent-deactivation="true">
        <p>vue-draggable-resizable</p>
      </vue-draggable-resizable>

         <vue-draggable-resizable axis="x" :w="100" :h="50" :y="20" :x="150" :parent="true" :active="true" :handles="['ml','mr']" :prevent-deactivation="true" >
        <p>vue-draggable-resizable</p>
      </vue-draggable-resizable>

         <vue-draggable-resizable axis="x" :w="100" :h="50" :y="20" :x="300" :parent="true" :handles="['ml','mr']" :active="true" :prevent-deactivation="true" >
        <p>vue-draggable-resizable</p>
      </vue-draggable-resizable>

    </div>
    <div style="height: 500px; width: 500px; border: 1px solid red; position: relative;">
      <vue-draggable-resizable axis="x" :w="20" :h="50" :y="20" :x="0" data-id="a1" :collision="true" :min-width="20" :handles="['ml','mr']" :active="true" :prevent-deactivation="true">
        <p>vue-draggable-resizable2</p>
      </vue-draggable-resizable>

         <vue-draggable-resizable axis="x" :w="20" :h="50" :y="20" :x="0" data-id="a2" :collision="true" :min-width="20" :active="true" :handles="['ml','mr']" :prevent-deactivation="true" >
        <p>vue-draggable-resizable2</p>
      </vue-draggable-resizable>

         <vue-draggable-resizable axis="x" :w="100" :h="50" :y="20" :x="20" data-id="a3" :collision="true" :min-width="20" :handles="['ml','mr']" :active="true" :prevent-deactivation="true" >
        <p>vue-draggable-resizable2</p>
      </vue-draggable-resizable>

    </div>
  </div>
</template>

<script>
import VueDraggableResizable from './components/vue-draggable-resizable'
import './components/vue-draggable-resizable.css'

export default {
  name: 'app',
  components: {
    VueDraggableResizable
  },
  data: () => ({
    myX: 100,
    myWidth: 400
  })
  // mounted () {
  //   const me = this
  //   setTimeout(function () {
  //     me.myX = 390
  //   }, 5000)

  //   setTimeout(function () {
  //     me.myWidth = 100
  //   }, 1000)
  // }
}
</script>

<style>
  .vdr {
    border: 1px dashed black;
  }
</style>
