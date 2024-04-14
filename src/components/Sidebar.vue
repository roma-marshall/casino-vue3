<template>
  <aside id="logo-sidebar" class="fixed pt-4 top-0 left-0 z-50 h-screen transition-transform -translate-x-full bg-white border-r border-gray-200 sm:translate-x-0 dark:bg-gray-800 dark:border-gray-700" aria-label="Sidebar">
    <div class="h-full px-3 pb-4 overflow-y-auto bg-white dark:bg-gray-800">
      <button @click="showMenu()" data-drawer-target="logo-sidebar" data-drawer-toggle="logo-sidebar" aria-controls="logo-sidebar" type="button" class="inline-flex items-center p-2 text-sm text-gray-500 rounded-lg sm:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600">
        <span class="sr-only">Open sidebar</span>
        <svg aria-hidden="true" class="flex-none w-6 h-6" fill="#6A7280" viewBox="0 0 24 24">
          <use xlink:href="../assets/icons/icons.svg#x" />
        </svg>
      </button>
      <ul class="space-y-2 font-medium">
        <li>
          <a href="#" class="flex flex-col items-center p-2 text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 group">
            <svg aria-hidden="true" class="flex-none w-16 h-16 scale-75">
              <use xlink:href="../assets/icons/icons.svg#slots" />
            </svg>
            <span>Slots</span>
          </a>
        </li>
        <li>
          <a href="#" class="flex flex-col items-center p-2 text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 group">
            <svg aria-hidden="true" class="flex-none w-16 h-16 scale-75">
              <use xlink:href="../assets/icons/icons.svg#live" />
            </svg>
            <span>Live</span>
          </a>
        </li>
        <li>
          <a href="#" class="flex flex-col items-center p-2 text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 group">
            <svg aria-hidden="true" class="flex-none w-16 h-16 scale-75" fill="#6A7280" viewBox="0 0 122.88 122.88">
              <use xlink:href="../assets/icons/icons.svg#bets" />
            </svg>
            <span>Bets</span>
          </a>
        </li>
        <li>
          <a href="#" class="flex flex-col items-center p-2 text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 group">
            <svg aria-hidden="true" class="flex-none w-16 h-16 scale-75" fill="none" viewBox="0 0 24 24">
              <use xlink:href="../assets/icons/icons.svg#bonus" />
            </svg>
            <span>Bonus</span>
          </a>
        </li>
        <li>
          <a href="#" class="flex flex-col items-center p-2 text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 group">
            <svg aria-hidden="true" class="flex-none w-16 h-16 scale-75" fill="none" viewBox="0 0 24 24">
              <use xlink:href="../assets/icons/icons.svg#ranking" />
            </svg>
            <span>Ranking</span>
          </a>
        </li>
        <li>
          <a href="#" class="flex flex-col items-center p-2 text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 group">
            <svg aria-hidden="true" class="flex-none w-16 h-16 scale-75" fill="none" viewBox="0 -0.5 25 25">
              <use xlink:href="../assets/icons/icons.svg#refs" />
            </svg>
            <span>Referrals</span>
          </a>
        </li>
        <li>
          <a href="#" class="flex flex-col items-center p-2 text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 group">
            <svg aria-hidden="true" class="flex-none w-16 h-16 scale-75" fill="#6A7280" viewBox="0 0 512 512">
              <use xlink:href="../assets/icons/icons.svg#support" />
            </svg>
            <span>Help</span>
          </a>
        </li>
      </ul>
    </div>
  </aside>
</template>

<script setup>
import { ref } from 'vue'

const showMenu = () => {
  document.querySelector('#logo-sidebar').classList.toggle('w-full')
  document.querySelector('#logo-sidebar').classList.toggle('-translate-x-full')
}
</script>