<template>
  <div class="main-board">
    <div class="board-row">
      <Gamebox 
        v-for="index in 10" 
        :key="index"
      />
    </div>
    <!--/* separate cols to either side */-->
    <div class="main-col">
      <div class="board-col">
        <Gamebox 
          v-for="index in 10" 
          :key="index"
        />
      </div>
      <div class="board-col">
        <Gamebox 
          v-for="index in 10" 
          :key="index"
        />
      </div>
    </div>
    <div class="board-row">
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
.main-board {
  width: 600px;
  margin: 0 auto 80px;
  display: flex;
  flex-direction: column;
}
.board-row {
  display: flex;
  flex-direction: row;
}
.board-row div {
  border-top: 1px solid #000;
  border-right: 1px solid #000;
  border-bottom: 1px solid #000;
}
.board-row div:first-child {
  border-left: 1px solid #000;
  width: 100px;
}
.board-row div:last-child {
  width: 100px;
}
.main-col {
  display: flex;
  justify-content: space-between;
}
.board-col {
  display: flex;
  flex-direction: column;
}
.board-col div {
  width: 98px;
  height: 50px;
  border-right: 1px solid #000;
  border-left: 1px solid #000;
  border-top: 1px solid #000;
  /*background: linear-gradient(to left, #fff 50%, #0000ff 50%);*/
}
.board-col div:first-child {
  border-top: none;
}
</style>