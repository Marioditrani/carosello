<script>
export default{
  data:()=> ({
    images :[
    "https://picsum.photos/id/1032/900/400",
    "https://picsum.photos/id/1033/900/400",
    "https://picsum.photos/id/1034/900/400",
    "https://picsum.photos/id/1035/900/400",
    "https://picsum.photos/id/1036/900/400",
    ]
  })
}


</script>

<template>
 <div class="carosello">
  <div class="carosello-container">
    <div class="carosello-item" v-for="image in images" :key="image">
      <img :src="image" />
    </div>
  </div>
  <div class="button">
    <div class="button-up">&#8593;</div>
    <div class="button-down">&#8595;</div>
  </div>
 </div>
</template>

<style scoped>
.carosello{
  display: flex;
  justify-content: center;
  gap: 30px;
}

.button{
  display: flex;
  justify-content: space-between;
  flex-direction: column;
}
.button-up, .button-down{
  font-size: 50px;
}
</style>
