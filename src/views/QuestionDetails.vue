<script setup>
import UpArrow from '../components/icons/UpArrow.vue'
import DownArrow from '../components/icons/DownArrow.vue'
import { ref } from 'vue'

let val = ref(0);

let upvote = () => {
    val.value++
}

let doenvote = () => {
    if (!val.value == 0) {
       val.value-- 
    }
}
</script>

<template>
  <div class="ques-detail">
    <div>
    <h1>How to make sibling div element visible when list item is hovered on</h1>
    </div>
    <div class="block">
    <div class="width-4">
        <div class="up-arrow mar-60l"><button class="btn-style" @click="upvote"><UpArrow /></button></div>
        <div class="count-val">{{val}}</div>
        <div class="mar-16t mar-60l"><button class="btn-style" @click="doenvote"><DownArrow /></button></div>
    </div>
    <div class="text-div">
        <p>I have the following simple header component with navigation items, which when hovered on should add the following two css rules to the mega-menu div element so that it appears:</p>
    </div>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .ques-detail {
    min-height: 100vh;
    font-size: 13px;
  }
  .width-4 {
    width: 3%;
    display: inline-block;
  }
  .count-val {
    margin-top: 14px;
    font-size: 20px;
    text-align: center;
  }
  .up-arrow {
    height: 15px;
  }
  .mar-60l {
    margin-left: 68px;
  }
  .mar-16t {
        margin-top: -16px;
  }
  .btn-style {
    border: none;
    background: none;
  }

  .text-div {
    width: 50%;
    display: inline-block;
    font-size: 15px;
        margin-left: 22px;
  }

  .block {
        display: block;
  }

}
</style>
