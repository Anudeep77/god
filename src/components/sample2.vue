<template>
<div>
  <h2>sadara</h2>
  <p>sadara</p>
 </div>
</template>
<script>
export default{
name: "sample2",
   data() {
    return {
    title:"anudeep"
 
  }
},
methods:{
changeTitle: function(ev){
this.title= ev.target.value;
}
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color:blue;
  

}

</style>