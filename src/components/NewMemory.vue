<template>
  <div>
      <h1>Yeni Ani | componenti</h1>
      <button @click="counter++">Add</button>
      <p>{{ counter }}</p>
  </div>
</template>


<script>
export default{
    data:function(){
        return{
            counter:0
        }
    },
    destroyed(){
        console.log("Destroyed!!!");
    },
    activated(){
        console.log("Activated!!!")

    },
    deactivated(){
        console.log("Deactivated!!!")
    }

}
</script>