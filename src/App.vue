<script setup lang="ts">
import Snake from "./components/Snake.vue";
</script>

<template>
  <div class="snake">
    <div class="flex">
      <Snake />
      <div class="show">
        <div class="code">
          // use keyboard <br />// arrows to play
          <div class="flex ac">
            <div class="dir-box">&#9650;</div>
            <div class="flex">
              <div class="dir-box">&#x25c0;</div>
              <div class="dir-box">&#9660;</div>
              <div class="dir-box">&#9654;</div>
            </div>
          </div>
        </div>
        <div></div>
      </div>
    </div>
    <div class="icon icon1"></div>
    <div class="icon icon2"></div>
    <div class="icon icon3"></div>
    <div class="icon icon4"></div>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
.snake {
  position: relative;
  padding: 35px 30px;
  box-sizing: border-box;
  background: linear-gradient(
    150.26deg,
    rgba(23, 85, 83, 0.7) 1.7%,
    rgba(67, 217, 173, 0.091) 81.82%
  );
  border: 1px solid #0c1616;
  box-shadow: inset 0px 2px 0px rgba(255, 255, 255, 0.3);
  backdrop-filter: blur(32px);

  border-radius: 8px;
}
.icon {
  position: absolute;
  width: 13px;
  height: 13px;
  background: radial-gradient(
    73.08% 73.08% at 50% 26.92%,
    #196c6a 15.1%,
    #114b4a 100%
  );
  border-radius: 50%;
  box-shadow: 2px 2px 4px #0d4341, inset 0px 1px 2px #1a8277;
}
.icon1 {
  left: 12px;
  top: 12px;
}
.icon2 {
  right: 12px;
  top: 12px;
}
.icon3 {
  left: 12px;
  bottom: 12px;
}
.icon4 {
  right: 12px;
  bottom: 12px;
}
.flex {
  display: flex;
}

.code {
  background: rgba(1, 20, 35, 0.19);
  border-radius: 8px;
  padding: 15px 13px;
  width: 186px;
  font-weight: 450;
  font-size: 14px;
  line-height: 18px;
}
.show {
  margin-left: 24px;
}
.dir-box {
  margin-top: 2px;
  width: 50px;
  height: 30px;
  line-height: 30px;
  background: #010c15;
  border: 1px solid #1e2d3d;
  border-radius: 8px;
  align-items: center;
  justify-content: center;
}
.ac {
  margin-top: 30px;
  flex-direction: column;
  align-items: center;
}
</style>
