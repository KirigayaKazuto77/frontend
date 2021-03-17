<template>
<Navbar/>
<br>

<div class="mothercontainer">

    <div class="container1">

        <div class="vertical-menu">
            <a v-on:click="isclicked = 1" href="#mainmenu">Link 1</a>
            <a v-on:click="isclicked = 2" href="#mainmenu">Link 2</a>
            <a v-on:click="isclicked = 3" href="#mainmenu">Link 3</a>
            <a v-on:click="isclicked = 4" href="#mainmenu">Link 4</a>
            <a v-on:click="isclicked = 5" href="#mainmenu">Link 5</a>
        </div>

        <div v-show="isclicked == 1" class="content">
            <Comp_Reg_Info/>
        </div>
        <div v-show="isclicked == 2" class="content">
            <Comp_Reg_Comp/>
        </div>
        <div v-show="isclicked == 3" class="content">
            <h1>Table Content 3</h1>
        </div>
        <div v-show="isclicked == 4" class="content">
            <h1>Table Content 4</h1>
        </div>
        <div v-show="isclicked == 5" class="content">
            <h1>Table Content 5</h1>
        </div>

    </div>

</div>
</template>



<script>

import Navbar from '@/components/Navbar.vue'
import Comp_Reg_Info from '@/components/Comp_Reg_Info.vue'
import Comp_Reg_Comp from '@/components/Comp_Reg_Comp.vue'

export default {
  name: 'MainMenu',
  components: {
    Navbar,
    Comp_Reg_Info,
    Comp_Reg_Comp
  }
}

</script>



<style scoped>

.mothercontainer{
    height: 700px;
    background-color: rgba(255, 255, 255, 0.2);
}

.container1 {
    height: 100%;
    display: grid;
    grid-template-columns: 25% 75%;
    background-color: white;
    padding: 0px;
}

.content{
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    border: 1px solid rgba(0, 0, 0, 0.8);
}

.vertical-menu {
  background-color: rgb(228, 228, 228);
  width: 100%;
  height: 100%;
}

.vertical-menu a {
  background-color: rgb(228, 228, 228);
  color: black;
  display: block;
  padding: 12px;
  text-decoration: none;
}

.vertical-menu a:hover {
  background-color: #4CAF50;
}

</style>
