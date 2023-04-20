<script setup>

const data =  [
    {
       "title": "Clean the kitchen",
       "description": "Mop the floor, wipe the countertop and don't forget to take out the trash!"
    },
    {
       "title": "Call Mom",
       "description": "It's her birthday!"
    },
    {
       "title": "Water flowers",
       "description": "They need water, or they will die."
    },
    {
        "title": "Clean the kitchen",
        "description": "Mop the floor, wipe the countertop and don't forget to take out the trash!"
     },
     {
        "title": "Call Mom",
        "description": "It's her birthday!"
     },
     {
        "title": "Water flowers",
        "description": "They need water, or they will die."
     },
     {
        "title": "Clean the kitchen",
        "description": "Mop the floor, wipe the countertop and don't forget to take out the trash!"
     },
     {
        "title": "Call Mom",
        "description": "It's her birthday!"
     },
     {
        "title": "Water flowers",
        "description": "They need water, or they will die."
     }
 ] 
</script>

<template>
<div class="main-div">
<button class="btn-style" @click="$router.push('/ask-question')">Ask Question</button>
<div>
<div class="card-view" v-for="item in data" :key="item.id">
  <a href="/question-details"><div class="tittle-clr">{{item.title}}</div></a>
  <div>{{item.description}}</div>
</div>
</div>
</div>
 
</template>


<style>
.main-div {
    display: block;
    margin: 35px auto;
    padding: 20px;
}

.card-view {
   height: 75px;
    font-size: 18px;
    margin: auto;
    border-top: 1px solid #00000038;
    padding: 10px;
}
.card-view:first-child {
   margin-top: 35px;
}
.btn-style {
   width: 104px;
    height: 34px;
    background: #1010e4c2;
    color: white;
    border: none;
    float: right;
}
.tittle-clr {
   color: hsl(206,100%,52%);
}
</style>