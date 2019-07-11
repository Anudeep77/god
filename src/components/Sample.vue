<template>
  <div class="hello">
    <h1>{{name}}</h1>
    <table v-if="isVisible">
    <tr>
    <th>name</th>
    <th>age</th>
    </tr>
    <tr v-for="Item in person">
    <td>{{Item.name}}</td>
    <td>{{Item.age}}</td>
    </tr>
    </table>
    <button @click="abc">click me</button>
             
  </div>
</template>

<script>
export default{
name: "sample",
   data() {
    return {
    person:[{name: "Anudeep" ,age: 21},{name: "mahesh",age: 26},{name: "dinesh",age: 27}],
    isVisible:true
  }
},
methods:{
abc: function(){
   this.isVisible=!this.isVisible
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
