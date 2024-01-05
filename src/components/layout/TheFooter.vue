<script setup lang="ts">
import SeparatorTripleLine from '@/components/separator/TripleLine.vue'
import SVGLogo from '@/components/SVGLogo.vue';

//TODO router link vuerouter instead of Anchor  
</script>

<template>
  <SeparatorTripleLine class="absolute bottom-50 md:bottom-15" />
  <footer data-test="footer"
    class="flex flex-col md:flex-row justify-between items-center h-50 md:h-15 px-2 md:px-4 py-4">
    <SVGLogo class="h-9 w-9 order-last md:order-first" />
    <nav class="flex flex-col md:flex-row justify-center items-center space-y-2 md:space-y-0 w-full text-sm">
      <a href='/privacy-and-permissions'>Privacy Permissions</a>
      <span class="hidden md:inline m-4">|</span>
      <a href='/dei'>DEI</a>
      <span class="hidden md:inline m-4">|</span>
      <a href='/code-of-conduct'>Code of Conduct</a>
    </nav>
    <div class="min-w-fit text-sm" data-test="footer-nav-text">&copy; {{ new Date().getFullYear() }} Schrödinger Hat</div>
  </footer>
</template>
