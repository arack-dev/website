<template>
  <div class="slider-thumb"></div>
  <div class="slider-thumb two"></div>
  <div class="slider-thumb"></div>
  <div class="slider-thumb"></div>
  <div class="slider-thumb"></div>
  <div class="slider-thumb"></div>
  <div class="slider-thumb"></div>
  <div class="slider-thumb"></div>
  <div class="slider-thumb"></div>
</template>

<style scoped>
body {
  height: 100vh;
  background: linear-gradient(90deg,#e52e71,#ff8a00);
}

.slider-thumb {
  position: fixed;
  content: "";
  left: -15%;
  top: 20%;
  width: 450px;
  height: 450px;
  background: #434343;
  background: linear-gradient(to left, var(--color-primary), var(--color-secondary));
  border-radius: 62% 47% 82% 35% / 45% 45% 80% 66%;
  will-change: border-radius, transform, opacity;
  animation: sliderShape 5s linear infinite;
  display: block;
  z-index: -1;
  -webkit-animation: sliderShape 5s linear infinite;

  &:nth-child(3) {
    left: 75%;
    top: 45%;
  }
  &:nth-child(4) {
    width: 150px;
    height: 150px;
    left: 15%;
    top: 10%;
  }
  &:nth-child(5) {
    width: 150px;
    height: 150px;
    left: 70%;
    top: 20%;
  }
  &:nth-child(6) {
    width: 600px;
    height: 350px;
    left: 25%;
    top: 80%;
  }
  &:nth-child(7) {
    width: 50px;
    height: 50px;
    left: 62%;
    top: 70%;
  }
  &:nth-child(8) {
    width: 450px;
    height: 450px;
    left: 40%;
    top: -25%;
  }
  &:nth-child(9) {
    width: 80px;
    height: 80px;
    left: 12%;
    top: 70%;
  }
}
.two {
  width: 50px;
  height: 50px;
  left: 50%;
  top: 45%;
}
@keyframes sliderShape{
  0%,100%{
    border-radius: 42% 58% 70% 30% / 45% 45% 55% 55%;
    transform: translate3d(0,0,0) rotateZ(0.01deg);
  }
  34%{
    border-radius: 70% 30% 46% 54% / 30% 29% 71% 70%;
    transform:  translate3d(0,5px,0) rotateZ(0.01deg);
  }
  50%{
    transform: translate3d(0,0,0) rotateZ(0.01deg);
  }
  67%{
    border-radius: 100% 60% 60% 100% / 100% 100% 60% 60% ;
    transform: translate3d(0,-3px,0) rotateZ(0.01deg);
  }
}
</style>