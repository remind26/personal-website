<template>
  <main
    class="mt-10 md:mt-1 flex flex-col-reverse gap-8 items-center md:flex-row md:gap-16 md:justify-center min-h-[65vh] md:min-h-[80vh]">
    <div class="space-y-2 text-center md:text-left px-10">
      <p class="text-green-600">Hey there! I'm</p>
      <h1 class="text-4xl font-bold md:text-5xl text-gray-900 fadein-up">Muhammad Ridhwan Ramadhan</h1>
      <div class="py-2">
        <h1 class="blinking text-xl font-semibold text-transparent bg-clip-text bg-gradient-to-r from-green-400 to-green-900 md:text-2xl fadein-up">
          Web Developer
        </h1>
      </div>
      <p class="text-gray-900 pr-4 fade-in-from-left">Welcome to my personal website! Dive in to explore my journey<span class="wave">👋🏼</span></p>
      <br>
      <div class="flex justify-center md:justify-start space-x-3">
        <a href="https://www.linkedin.com/in/muhammadridhwanramadhan/" class="social-icon transition duration-300 ease-in-out hover:scale-110">
          <i class="fab fa-linkedin text-blue-600 text-2xl"></i>
        </a>
        <a href="https://instagram.com/ridhwanr._" class="social-icon transition duration-300 ease-in-out hover:scale-110">
          <i class="fab fa-instagram text-pink-600 text-2xl"></i>
        </a>
        <a href="https://wa.me/6287727732608" class="social-icon transition duration-300 ease-in-out hover:scale-110">
          <i class="fab fa-whatsapp text-green-600 text-2xl"></i>
        </a>
      </div>
    </div>
    <div class="flex justify-center md:justify-start fadein-right"><img alt="avatar" fetchpriority="high" width="300" height="300" decoding="async" data-nimg="1"
        class="w-10/12 md:h-auto rounded-full pict" src="../assets/profile.png">
    </div>
  </main>
</template>

<script>
export default {
  name: 'HomeView',
  data() {
    return {
      txt: 'Web Developer',
    };
  }
}
</script>

<style>
body {
  overflow-y: scroll;
  overflow-x: hidden;
}

.blinking {
  animation: blink 1s step-start infinite;
}

@keyframes blink {
  50% {
    opacity: 0;
  }
}

.typewrite>.wrap {
  border-right: 0.08em solid #000; /* Changed to black */
}

.wave {
  animation-name: wave-animation;
  animation-duration: 2.5s;
  animation-iteration-count: infinite;
  transform-origin: 70% 70%;
  display: inline-block
}

@keyframes wave-animation {
  0% {
    transform: rotate(0deg)
  }

  10% {
    transform: rotate(14deg)
  }

  20% {
    transform: rotate(-8deg)
  }

  30% {
    transform: rotate(14deg)
  }

  40% {
    transform: rotate(-4deg)
  }

  50% {
    transform: rotate(10deg)
  }

  60% {
    transform: rotate(0deg)
  }

  to {
    transform: rotate(0deg)
  }
}

.pict {
  box-shadow: 0px 0px 73px -9px rgba(72, 187, 120, 0.44); /* Updated to green */
  -webkit-box-shadow: 0px 0px 73px -9px rgba(72, 187, 120, 0.44);
  -moz-box-shadow: 0px 0px 73px -9px rgba(72, 187, 120, 0.44);
}

.fadein-up {
  opacity: 0;
  animation-name: fadeInUp;
  animation-duration: 0.5s;
  animation-fill-mode: forwards;
  animation-delay: 500ms;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translate3d(0, 100%, 0);
  }

  to {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

.fade-in-from-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
  animation-delay: 500ms;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadein-right {
  opacity: 0;
  animation: fadeInRight 0.5s ease-out forwards;
  animation-delay: 500ms;
}

@keyframes fadeInRight {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadein-bot {
  opacity: 0;
  animation: fadeInBot 0.5s forwards;
}

@keyframes fadeInBot {
  from {
    opacity: 0;
    transform: translate3d(0, -100%, 0);
  }

  to {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

.fadein-1 {
  animation-delay: 200ms;
}
.fadein-2 {
  animation-delay: 400ms;
}
.fadein-3 {
  animation-delay: 600ms;
}
.fade-500 {
  animation-delay: 500ms;
}

.social-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 40px; /* Default size */
  height: 40px;
  border-radius: 50%;
  background-color: white;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s, box-shadow 0.3s;
}

.social-icon:hover {
  transform: scale(1.1);
  box-shadow: 0px 8px 10px rgba(0, 0, 0, 0.2);
}

@media (min-width: 768px) {
  .social-icon {
    width: 35px;
    height: 35px;
  }
}


@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadein-left-1 {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
  animation-delay: 200ms;
}

.fadein-left-2 {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
  animation-delay: 400ms;
}

.fadein-left-3 {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
  animation-delay: 600ms;
}
</style>
