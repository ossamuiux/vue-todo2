<script setup>
// vue3 컴포지션 api 가져오기
// 객체구조분해로 필요한 함수 불러오기
import { reactive, computed } from 'vue';

// 할일 삭제
function deleteItem(id) {
  // id에 맞는 아이템을 찾기
  const itemToDelete = data.items.find((item) => item.id === id);

  // 삭제할 아이템의 위치 찾기
  const idx = data.items.indexOf(itemToDelete);

  // splice(시작위치, 삭제갯수)
  data.items.splice(idx, 1);
}

function test() {
  console.log('11');
}
test();

function test222() {
  console.log('22');
}
test222();

function test333() {
  console.log('33');
}
test333();
</script>

<template>
  <main class="Test">
    <h1>Simple to-do list</h1>
  </main>
</template>

<style scoped></style>
