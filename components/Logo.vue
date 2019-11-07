<template>
  <div class="gluglogo">
    <img class='img' src="@/static/glug-logo.svg" alt="GLUG">
  </div>
</template>

<style>
.gluglogo {
  display: inline-block;
  animation: turn 2s linear forwards 1s;
  transform: rotateX(180deg);
  position: relative;
  overflow: visible;
  margin-top: 5vh;
  height: 150px; 
  margin-bottom: 5px;
}

@keyframes turn {
  100% {
    transform: rotateX(0deg);
  }
}

@media only screen and (max-width: 767px){

.img {
  transform: scale(0.8,0.8);
  transform: translate(3%,-15%);
}
}
@media only screen and (min-width: 768px){

.img {
  transform: scale(0.9,0.9);
  transform: translate(3%,-15%);
}
}


</style>
