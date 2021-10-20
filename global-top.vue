<template>
  <footer v-if="$slidev.nav.currentRoute.meta.section === 1" class="absolute bottom-0 left-0 p-2 text-xs" style="opacity: 0.8;">
    1. Diagrams and NIFs
  </footer>
  <footer v-if="$slidev.nav.currentRoute.meta.section === 2" class="absolute bottom-0 left-0 p-2 text-xs" style="opacity: 0.8;">
    2. Navigations and Code
  </footer>
  <footer v-if="$slidev.nav.currentRoute.meta.section === 3" class="absolute bottom-0 left-0 p-2 text-xs" style="opacity: 0.8;">
    3. Other Stuff
  </footer>
  <footer
    v-if="$slidev.nav.currentLayout !== 'cover'"
    class="absolute bottom-0 right-0 p-2"
  >
    {{ $slidev.nav.currentPage }}.{{ $slidev.nav.clicks }} / {{ $slidev.nav.total }}
  </footer>
</template>
