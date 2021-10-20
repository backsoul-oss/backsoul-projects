<template>
  <div class="flex justify-center items-center w-full h-screen  z-10">
    <div class="flex justify-center flex-col items-center 2xl:flex-row 2xl:justify-between 2xl:w-flex 2xl:items-center w-full">
      <img :src="require(`~/assets/img/character-intro.png`)" class="image 2xl:order-2 sm:w-64 md:w-96" draggable="false"/>
      <div class="2xl:order-1">
        <h1 class="font-bold md:text-4xl text-welcome sm:text-base sm:text-center">Welcome enthusiastic!</h1>
        <p class="md:text-2xl text-center 2xl:text-left sm:text-base">Daniel Sarmiento FullStack developer.</p>
        <div class="mt-2 flex justify-center gap-5 2xl:justify-start">
          <a href="https://twitter.com/backsoul_" target="_blank">
            <svgicon
              name="twitter"
              width="30"
              color="#fffff"
              class="fill-current hover:text-orange"
            ></svgicon>
          </a>
          <a href="https://github.com/backsoul" target="_blank">
            <svgicon
              name="github"
              width="30"
              color="#fffff"
              class="fill-current hover:text-orange"
            ></svgicon>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.text-welcome {
  width: fit-content;
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: 0.15em solid orange; /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: 0.15em; /* Adjust as needed */
  animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
}

@keyframes typing {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}

@keyframes blink-caret {
  from,
  to {
    border-color: transparent;
  }
  50% {
    border-color: orange;
  }
}

.image {
  animation: float 5s infinite;
}

@keyframes float {
  0% {
    transform: translatey(0px);
  }
  50% {
    transform: translatey(-10px);
  }
  100% {
    transform: translatey(0px);
  }
}
</style>
