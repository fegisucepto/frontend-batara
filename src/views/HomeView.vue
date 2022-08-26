<template>
  <section>
    <NavbarPage />
    <FooterPage />
  </section>
</template>
<script>
import NavbarPage from '@/components/Navbar'
import FooterPage from '@/components/Footer'

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
    FooterPage
  }
}
</script>
<style></style>
