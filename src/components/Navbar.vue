<template>
  <nav class="fixed w-full z-30 top-0 text-white">
    <div
      class="w-full container mx-auto flex flex-wrap items-center justify-between mt-0 py-2"
    >
      <div class="pl-4 flex items-center">
        <a
          class="text-white no-underline hover:no-underline font-bold text-4xl"
          href="#"
        >
          <i class="fak fa-liskadev"></i>
        </a>
      </div>
      <div
        class="flex-grow flex items-center w-auto mt-0 bg-transparent p-4 lg:p-0 z-20"
      >
        <ul class="list-reset flex justify-end flex-1 items-center">
          <li class="mr-3">
            <a
              class="inline-block py-2 px-4 font-bold no-underline"
              href="https://github.com/Webess"
              ><i class="fab fa-github"></i
            ></a>
          </li>
          <li class="mr-3">
            <a
              class="inline-block py-2 px-4 font-bold no-underline"
              href="https://www.linkedin.com/in/tomliska/"
              ><i class="fab fa-linkedin"></i
            ></a>
          </li>
          <li class="mr-3">
            <a
              class="inline-block py-2 px-4 font-bold no-underline"
              href="https://www.instagram.com/tomas_liska/"
              ><i class="fab fa-instagram"></i
            ></a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>
