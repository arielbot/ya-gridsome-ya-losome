<template>
  <div class="main-board">
    <div class="top-row">
      <Gamebox 
        v-for="index in 10" 
        :key="index"
      />
    </div>
    <div class="left-col">
      <Gamebox 
        v-for="index in 10" 
        :key="index"
      />
    </div>
  </div>
</template>

<script>
import Gamebox from '~/components/Gamebox.vue'

export default {
  components: {
    Gamebox
  }
}
</script>

<style>
.top-row {
  display: flex;
  flex-direction: row;
}
.top-row div:first-child, .top-row div:last-child {
  width: 200px;
}
.left-col {
  display: flex;
  flex-direction: column;
}
.left-col div {
  width: 192px;
  height: 100px;
}
</style>