<script setup lang="ts">
import SeparatorTripleLine from '@/components/separator/TripleLine.vue'
import LogoAnimated from '@/components/buttons/LogoAnimated.vue'
import SVGLogo from '@/components/SVGLogo.vue';

//TODO router link vuerouter instead of Anchor  
</script>

<template>
  <footer class="relative h-16" data-test="footer">
    <SeparatorTripleLine class="absolute bottom-16" />
    <div class=" flex justify-between items-center w-full h-full px-2 py-5 mx-auto">
      <SVGLogo class="h-9 w-9" />
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

  </footer>
</template>
