<template>
<div>
  <b-navbar toggleable="lg" type="dark" variant="dark">
    <NuxtLink class="navbar-brand" to="/">Firengii</NuxtLink>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-navbar-nav>
        <NuxtLink to="/products" class="nav-link"
            >Products <span class="sr-only">(current)</span></NuxtLink
          >
        <NuxtLink to="/my-items" class="nav-link"
            >My Items <span class="sr-only">(current)</span></NuxtLink
          >
      </b-navbar-nav>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
</style>
