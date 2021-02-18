<template>
  <div class="pageCon">
      <h1>Treixatek</h1>
  </div>
</template>

<script>
export default {
  head(){
    return{
      title: "About Us | Treixatek",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Learn about the indie game development studio Treixatek and see our story"
        }
      ]
    }
  }
}
</script>

<style>

/* PAGE ANIMATIONS */
.pageCon {
  width: 100%;
  animation-timing-function: ease-out;
  animation: transitionIn 0.5s;
}
@keyframes transitionIn {
  from{
    opacity: 0;
    
    transform: translateY(5vh);
  }

  to {
    opacity: 1;
    
    transform: translateY(0);
  }
}
</style>