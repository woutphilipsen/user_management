<template>
  <main>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="#">platonic solids</a>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarNavAltMarkup"
        aria-controls="navbarNavAltMarkup"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <inertia-link href="/users" class="nav-item nav-link active">
            Home
            <span class="sr-only">(current)</span>
          </inertia-link>
          <inertia-link class="nav-item nav-link" href="/about">About</inertia-link>
          <inertia-link class="nav-item nav-link" href="/contact">Contact</inertia-link>
        </div>
      </div>
    </nav>
    <article>
      <slot />
    </article>
  </main>
</template>

<script>
export default {
    inject: ['page'],
}
</script>