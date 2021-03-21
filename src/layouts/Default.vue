<template>
  <div class="w-full bg-gray-800">
    <div class="max-w-5xl mx-auto">
      <header class="flex text-white justify-between px-4 py-8 ">
        <strong>
          <!-- <g-link to="/">{{ $static.metadata.siteName }}</g-link> -->
          <g-link to="/" class="text-5xl">Gridsome Test</g-link>
        </strong>
        <nav class="nav space-x-4">
          <g-link class="nav__link" to="/">Home</g-link>
          <g-link class="nav__link" to="/about/">About</g-link>
          <g-link class="nav__link" to="/platzhalter/">Seite über Platzhalter</g-link>
        </nav>
      </header>
      <slot/>
    </div>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
