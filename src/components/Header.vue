<template>
  <div
    class="leading-normal tracking-normal text-white bg-[url('../src/assets/images/bg.jpg')] bg-bottom bg-cover rounded-bl-[3rem] sm:rounded-bl-[5rem]"
  >
    <div
      class="bg-gradient-to-r from-blue-700 via-blue-700 rounded-bl-[3rem] sm:rounded-bl-[5rem] relative"
    >
      <div
        class="container max-w-[90%] min-h-[350px] xs:min-h-[300px] mx-auto flex flex-wrap flex-row items-start xs:items-center"
      >
        <div class="flex flex-col w-full justify-center items-start text-left">
          <div class="flex flex-col pt-10 sm:pt-0">
            <h1
              class="text-6xl sm:text-7xl font-bold leading-[60px] text-center xs:text-left"
            >
              Tomáš Líška
            </h1>
            <h2
              class="leading-normal tracking-[0.2em] text-xl text-center xs:text-left xs:self-end uppercase font-bold text-blue-300"
            >
              Full-stack developer
            </h2>
          </div>
        </div>
      </div>
      <Technologies />
    </div>
  </div>
</template>

<script>
import Technologies from './Technologies.vue'
export default {
  name: 'Header',
  components: {
    Technologies,
  },
}
</script>
