<template>
  <div class="mb-10" v-if="data">
    <h4 class="text-2xl font-bold text-blue-700">
      <a
        class="group inline-block py-2 font-semibold leading-[30px] relative hover:text-black"
        :href="data.url"
        target="_blank"
        rel="noopener noreferrer"
        >{{ data.title }}
        <div
          class="w-[78px] h-[3px] bg-blue-300 absolute left-0 group-hover:left-2 transition-all duration-600"
        ></div>
      </a>
    </h4>
    <strong class="block my-3"
      >{{ data.year_from }} - {{ data.year_to }}</strong
    >
    <p class="leading-6">
      {{ data.description }}
    </p>
  </div>
</template>

<script>
export default {
  name: 'Experience',
  props: ['data'],
}
</script>
