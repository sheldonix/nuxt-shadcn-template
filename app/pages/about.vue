<template>
  <div class="container mx-auto max-w-5xl px-6 py-16">
    <!-- Header Section -->
    <section class="text-center mb-20">
      <h1 class="text-5xl font-bold mb-6">About</h1>
      <p class="text-muted-foreground text-xl max-w-2xl mx-auto leading-relaxed">
        About page content
      </p>
    </section>

    <!-- Back to Home -->
    <section class="text-center">
      <Button as-child variant="outline" size="lg">
        <NuxtLink to="/">Back to Home</NuxtLink>
      </Button>
    </section>
  </div>
</template>
