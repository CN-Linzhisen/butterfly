<template>
  <svg viewBox="0 0 340 333">

    <path
      class="path" stroke="#303" fill="#fff" stroke-width="4" d="M116 129C118.802 97.1511 125.151 67.8105 144 64.5C166.509 65.9142 81.1119 135.818 54 125C32.539 114.873 53.5958 74.6936 71.5 76.5C86.965 80.6497 70.2354 93.0991 50 92C30.928 80.5257 40.8068 68.4202 24.5 59.5C-2.46527 47.0615 -4.47938 40.176 7.49999 28C24.3788 13.5279 37.2346 13.2517 62 17C101.51 25.3682 112 59.5 98 59.5C84 59.5 97.5493 -0.165897 127 0.500009C143.126 2.47766 138.333 18.4076 127 43"
    />

  </svg>
</template>

<style scoped>
.path {
  stroke-dasharray: 1000;
  stroke-dashoffset: 1000;
  animation: dash 5s linear infinite;
}

.dark .path {
  stroke: #fdfdfd;
  fill: #000;
}
@keyframes dash {
  to {
    stroke-dashoffset: 0;
  }
}

@media (prefers-reduced-motion) {
  .path1 {
    animation: none !important;
    stroke-dasharray: unset !important;
  }
}
@media print {
  .path1 {
    animation: none !important;
    stroke-dasharray: unset !important;
  }
}
@keyframes grow {
  0% {
    stroke-dashoffset: 1px;
    stroke-dasharray: 0 350px;
    opacity: 0;
  }
  10% {
    opacity: 1;
  }
  40% {
    stroke-dasharray: 350px 0;
  }
  85% {
    stroke-dasharray: 350px 0;
  }
  95%,
  to {
    stroke-dasharray: 0 350px;
  }
}
.path1 {
  stroke-dashoffset: 1px;
  stroke-dasharray: 350px 0;
  animation: grow 10s ease forwards infinite;
  transform-origin: center;
  stroke: #303030;
  animation-delay: 0s;
}
.dark .path1 {
  stroke: #fdfdfd;
}
</style>
