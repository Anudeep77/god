;lkj<template>
<div>
<p>{{sayHello()}}</p> 
<p><a v-bind:href=link>google</a></p>
<h1>{{title}}</h1>
<button @click="increase">click me</button>
<p>{{counter}}</p>
<p v-on:mousemove="coordinate">coordinates: {{x}} / {{y}}-<span v-on:mousemove.stop="">stop</span></p>
<button @click="changelink">click to change link</button>
<a :href="link"> link </a>
<h2 :style="{color:'yellow'}"> This is Anudeep </h2>
<h1 :style="{background:'blue'}"> hello World </h1>
<h1 :style="anu">Hi World</h1>
<h3 v-if="isvisible">welcome</h3>
<h3 v-show="isvisible">welcome to</h3>
<h1 v-if="isvisible">Anudeep</h1>
<h1 v-else="isvisile">dhoni</h1>
<h2 v-if="a==b">Anu</h2>
<h3 v-else>hi this is javascript</h3>

 </div>
</template>
<script>
export default{
name: "sample3",
   data() {
    return {
    title:"Hello World",
    link:"http://google.com",
    counter: 0,
    link:"http://facebook.com",
    isvisible:true,
    anu :{
    color:'pink',
    background:'red'
    },
    a:20,
    b:20,
    x:0,
    y:0
 
  }
},
methods:{
sayHello: function(){
	return this.title;
},
increase: function(){
  this.counter++;
  },
  changelink: function(){
  this.link = "http://yahoo.com";
  },
  coordinate:function(event){
this.x=event.clientX;
this.y=event.clientY;
  },

}
} 
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color:red;
  

}

</style>