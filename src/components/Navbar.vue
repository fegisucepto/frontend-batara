<template>
  <div class="container-fluid bg-light position-relative shadow">
    <nav
      class="navbar navbar-expand-lg bg-light navbar-light py-3 py-lg-0 px-0 px-lg-5"
      id="mainNav"
    >
      <div class="container px-4 px-lg-5">
        <a class="navbar-brand font-weight-bold text-secondary" href="/"
          ><img src="../assets/todo.png" alt="todo"
        /></a>
        <button
          type="button"
          class="navbar-toggler"
          data-toggle="collapse"
          data-target="#navbarCollapse"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div
          class="collapse navbar-collapse justify-content-between"
          id="navbarResponsive"
        >
          <div class="navbar-nav font-weight-bold mx-auto py-0">
            <ul class="navbar-nav ms-auto my-2 my-lg-0">
              <li class="nav-item">
                <a class="nav-link" href="/home"></a>
              </li>
            </ul>
          </div>
          <a
            class="btn btn-warning px-4 mr-2"
            href="/todo-items"
            role="button"
            >Add News</a
          >
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'NavbarPage'
}
</script>

<style></style>
