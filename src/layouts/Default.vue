<template>
  <div class="font-sans sm:mx-2 sm:p-2 lg:mx-auto container">
    <header class="header flex align-center justify-between pt-10">
      <strong>
        <g-link class="text-xl text-gray-600" to="/">{{ $static.metaData.siteName }}</g-link>
      </strong>
      <nav class="nav text-lg">
        <g-link class="mx-2 hover:text-gray-600" to="/">Home</g-link>
        <g-link class="mx-2 hover:text-gray-600" to="/about">About</g-link>
      </nav>
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>
