<script setup lang="ts">
import SeparatorTripleLine from '@/components/separator/TripleLine.vue'
import LogoAnimated from '@/components/buttons/LogoAnimated.vue'
</script>

<template>
  <footer class="relative" data-test="footer">
    <SeparatorTripleLine class="absolute bottom-16" />
    <div class="container flex justify-center pt-10 text-left">
      <div class="flex justify-between items-center w-full h-full px-2 mx-auto">
        <LogoAnimated />
        <div>
          <a href='/privacy-and-permissions'>Privacy Permissions</a>
          <span class="m-4">|</span>
          <a href='/dei'>DEI</a>
          <span class="m-4">|</span>
          <a href='/code-of-conduct'>Code of Conduct</a>
        </div>
        <nav>
          <span data-test="footer-nav-text">&copy;{{ new Date().getFullYear() }} Schrödinger Hat</span>
        </nav>
      </div>
    </div>
  </footer>
</template>
