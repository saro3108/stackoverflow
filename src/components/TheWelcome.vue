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
  <Card>
    <template #title> Simple Card </template>
    <template #content>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Inventore sed consequuntur error repudiandae numquam deserunt quisquam repellat libero asperiores earum nam nobis, culpa ratione quam perferendis esse, cupiditate neque
            quas!
        </p>
    </template>
</Card>
<button class="btn-style">Ask Question</button>
<div>
<div class="card-view" v-for="item in data" :key="item.id">
  <div class="tittle-clr">{{item.title}}</div>
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
    margin-right: 134px;
}
.tittle-clr {
   color: hsl(206,100%,52%);
}
</style>