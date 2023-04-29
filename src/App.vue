<template>
  <Header />
  <div class="container max-w-[90%] mx-auto py-10">
    <div
      class="grid overflow-hidden grid-cols-1 md:grid-cols-2 grid-rows-1 gap-10 2xl:gap-60"
    >
      <div class="w-full">
        <h3 class="text-5xl font-bold text-blue-700 mb-5">
          Pracovné skúsenosti
        </h3>
        <Experience
          v-for="experience in experiences"
          :key="experience.id"
          :data="experience"
        />
      </div>
      <div class="w-full">
        <div class="mb-10">
          <h3 class="text-5xl font-bold text-blue-700 mb-7">Kto som</h3>
          <p class="leading-6 mb-3 w-full">
            Webový vývojár, ktorý sa o weby zaujíma už od roku 2009. Prvý web
            som spravil už na základnej škole, kde som upravoval HTML kód
            webových stránok z generátorov. Počas strednej školy som sa viac
            zblížil s PHP, kde som programoval šablóny pre PHP-Fusion a
            WordPress.
          </p>
          <p class="leading-6 mb-3">
            Popri štúdiu na Univerzite Konštantína Filozofa v Nitre som objavil
            PHP framework Laravel, na ktorom som postavil viacero veľkých
            systémov. Medzi ne patrí napríklad fakturačný systém, HRM, správa
            skladu alebo kasting databáza. Momentálne pracujem ako programátor
            pre firmu Dajana Rodriguez, kde sa primárne venujem vývoju e-shopu a
            interných systémov firmy.
          </p>
          <p>
            Pokiaľ by ste so mnou chceli naviazať kontakt alebo rovno spoluprácu
            neváhajte ma kontaktovať!
          </p>
          <div
            class="grid overflow-hidden grid-cols-1 xl:grid-cols-2 grid-rows-1 mt-8 items-center"
          >
            <ul class="list-reset flex flex-col flex-1 text-2xl mb-10 xl:mb-0">
              <li class="flex items-center mb-2">
                <a class="group flex" href="mailto:mail@example.org">
                  <span
                    class="bg-blue-700 text-white text-2xl text-center w-12 h-12 p-2 rounded-bl-lg rounded-tr-lg block group-hover:rounded-br-xl group-hover:rounded-tl-xl group-hover:rounded-bl-none group-hover:rounded-tr-none"
                  >
                    <i class="fas fa-at"></i>
                  </span>
                  <span
                    class="inline-block py-2 font-semibold relative group-hover:text-blue-700 ml-5"
                    >mail@example.org
                    <div
                      class="w-[98px] h-[3px] bg-blue-300 absolute left-0 group-hover:left-2 transition-all duration-600"
                    ></div>
                  </span>
                </a>
              </li>
              <li class="flex items-center">
                <a class="group flex" href="tel:+421123456789">
                  <span
                    class="bg-blue-700 text-white text-2xl text-center w-12 h-12 p-2 rounded-bl-lg rounded-tr-lg block group-hover:rounded-br-xl group-hover:rounded-tl-xl group-hover:rounded-bl-none group-hover:rounded-tr-none"
                  >
                    <i class="fas fa-phone"></i>
                  </span>
                  <span
                    class="inline-block py-2 font-semibold relative group-hover:text-blue-700 ml-5"
                    >+421 123 456 789
                    <div
                      class="w-[98px] h-[3px] bg-blue-300 absolute left-0 group-hover:left-2 transition-all duration-600"
                    ></div>
                  </span>
                </a>
              </li>
            </ul>
            <ul class="list-reset flex lg:justify-end text-3xl text-center">
              <li class="mr-5">
                <a
                  class="bg-blue-700 text-white w-16 h-16 p-4 rounded-bl-xl rounded-tr-xl block hover:rounded-br-xl hover:rounded-tl-xl hover:rounded-bl-none hover:rounded-tr-none"
                  href="https://github.com/Webess"
                  ><i class="fab fa-github"></i
                ></a>
              </li>
              <li class="mr-5">
                <a
                  class="bg-blue-700 text-white w-16 h-16 p-4 rounded-bl-xl rounded-tr-xl block hover:rounded-br-xl hover:rounded-tl-xl hover:rounded-bl-none hover:rounded-tr-none"
                  href="https://www.linkedin.com/in/tomliska/"
                  ><i class="fab fa-linkedin-in"></i
                ></a>
              </li>
              <li>
                <a
                  class="bg-blue-700 text-white w-16 h-16 p-4 rounded-bl-xl rounded-tr-xl block hover:rounded-br-xl hover:rounded-tl-xl hover:rounded-bl-none hover:rounded-tr-none"
                  href="https://www.instagram.com/tomas_liska/"
                  ><i class="fab fa-instagram"></i
                ></a>
              </li>
            </ul>
          </div>
        </div>
        <div class="mb-3">
          <h4 class="text-xl font-bold text-blue-700 mb-3">Fakturačné údaje</h4>
          <p class="text-sm xs:w-4/6 md:w-5/6 xl:w-1/2">
            <strong>Mgr. Tomáš Líška</strong><br />
            Dlhá ulica 123<br />
            123 45 Mesto<br /><br />
            <strong>IČO:</strong> 12 345 678<br /><br />
            Fyzická osoba zapísaná v Živnostenskom registri Okresného úradu
            Bratislava od 1. apríla 1999, Číslo živnostenského registra: 123-45678
          </p>
        </div>
        <div>
          <h4 class="text-xl font-bold text-blue-700 mb-3">Bankové spojenie</h4>
          <p class="text-sm xs:w-4/6 md:w-5/6 xl:w-1/2">
            <strong>IBAN:</strong> SK12 3456 7890 1234 4567 8901<br />
            <strong>Číslo účtu:</strong> 1234567890/1234<br />
            <strong>BIC SWIFT:</strong> XXXXXXXX
          </p>
        </div>
      </div>
    </div>
  </div>
  <div class="bg-black text-white p-5">
    <div class="container max-w-[90%] mx-auto text-center">
      <a href="https://liska.dev">
        <img class="w-7 inline-block" src="../favicon.png" alt="Tomáš Líška" />
      </a>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Experience from './components/Experience.vue'

import experiences from './assets/data/experiences.json'

import { orderBy } from 'lodash'

export default {
  name: 'App',
  components: {
    Header,
    Experience,
  },
  data() {
    return {
      experiences: orderBy(experiences, 'id', 'desc'),
    }
  },
}
</script>
