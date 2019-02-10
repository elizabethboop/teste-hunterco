<template>
  <div>
    <nav
      class="navbar navbar-expand-md fixed-top color"
      style="border-bottom: 1px solid #e7e7e7 !important;"
    >
      <a
        class="navbar-brand color"
        href="#"
      >HunterConnect</a>

      <div
        id="navbarCollapse"
        class="collapse navbar-collapse"
      >
        <ul class="navbar-nav mr-auto">
          <li class="nav-item">
            <a
              class="nav-link color"
              href="#"
            >
              Vagas
            </a>
          </li>
        </ul>

        <form class="form-inline mt-2 mt-md-0">
          <input
            class="form-control mr-sm-2"
            type="text"
            placeholder="Buscar vagas"
            aria-label="Buscar vagas"
          >
          <button type="button" class="btn btn-secondary my-2 my-sm-0 fundo">Buscar</button>
        </form>
      </div>
    </nav>

    <nuxt />
  </div>
</template>

<style>
</style>
