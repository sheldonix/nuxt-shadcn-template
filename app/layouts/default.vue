<template>
  <div class="min-h-screen bg-background flex flex-col">
    <!-- Header -->
    <header class="border-b">
      <div class="container mx-auto max-w-6xl px-6 py-4">
        <div class="flex items-center justify-between">
          <NuxtLink to="/" class="flex items-center gap-2">
            <div class="w-10 h-10 bg-primary rounded-lg flex items-center justify-center">
              <Zap class="w-6 h-6 text-primary-foreground" />
            </div>
            <h1 class="text-2xl font-bold">Nuxt + shadcn-vue</h1>
          </NuxtLink>
          <div class="flex items-center gap-2">
            <ThemeToggle />
            <Button as-child variant="ghost" size="sm">
              <NuxtLink to="/about">About</NuxtLink>
            </Button>
            <Button variant="outline" size="sm">Documentation</Button>
            <Button size="sm">Get Started</Button>
          </div>
        </div>
      </div>
    </header>

    <!-- Main Content -->
    <main class="flex-1">
      <slot />
    </main>

    <!-- Footer -->
    <footer class="border-t">
      <div class="container mx-auto max-w-6xl px-6 py-6 text-center text-sm text-muted-foreground">
        Built with Nuxt and shadcn-vue
      </div>
    </footer>
  </div>
</template>

<script setup lang="ts">
import { Zap } from 'lucide-vue-next'
</script>
