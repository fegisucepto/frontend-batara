<template>
  <section>
    <NavbarPage />
    <Todo />
    <FooterPage />
  </section>
</template>
<script>
import NavbarPage from '@/components/Navbar'
import FooterPage from '@/components/Footer'
import Todo from '../components/Todo.vue'
// import HomePage from '@/components/HomePage'

export default {
  name: 'HomeView',
  metaInfo: {
    // if no subcomponents specify a metaInfo.title, this title will be used
    title: 'Todo',
    // all titles will be injected into this template
    titleTemplate: '%s |Todo'
  },
  components: {
    NavbarPage,
    FooterPage,
    // HomePage
    Todo
  }
}
</script>
<style></style>
