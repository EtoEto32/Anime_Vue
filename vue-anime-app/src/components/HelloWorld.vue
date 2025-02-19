<template>
  <div class="hello">
    <h1>
      <span class="wavy-text">え</span>
      <span class="wavy-text">っ</span>
      <span class="wavy-text">と</span>
      <span class="wavy-text">っ</span>
      <span class="wavy-text">と</span>
    </h1>
  </div>
</template>

<style scoped>
@keyframes wavy {
  0% { transform: translateY(0px) rotate(0deg); }
  25% { transform: translateY(-3px) rotate(3deg); }
  50% { transform: translateY(2px) rotate(-2deg); }
  75% { transform: translateY(-1px) rotate(1deg); }
  100% { transform: translateY(0px) rotate(0deg); }
}

.wavy-text {
  display: inline-block;
  animation: wavy 1s infinite ease-in-out;
  color: #50C878; /* エメラルドグリーン */
}

/* ランダムなタイミングで開始させる */
.wavy-text:nth-child(1) { animation-delay: 0s; }
.wavy-text:nth-child(2) { animation-delay: 0.2s; }
.wavy-text:nth-child(3) { animation-delay: 0.4s; }
.wavy-text:nth-child(4) { animation-delay: 0.1s; }
.wavy-text:nth-child(5) { animation-delay: 0.3s; }
</style>
