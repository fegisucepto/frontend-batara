<template>
  <section>
    <div>
      <Navbar />
      <div class="container-fluid pt-5 pb-5">
        <div class="container pt-5 pb-5">
          <div class="row">
            <div class="col-lg-12 mb-5">
              <div class="card border-0 shadow-sm pb-2">
                <HomePage
                  v-for="listhome in HomePage"
                  :key="listhome.id"
                  :data="listhome"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
      <FooterPage />
    </div>
  </section>
</template>

<script>
import server from '@/api'
import FooterPage from '@/components/Footer'
import Navbar from '../components/Navbar.vue'
import HomePage from '../components/HomePage.vue'

export default {
  name: 'ListHome',
  metaInfo: {
    // if no subcomponents specify a metaInfo.title, this title will be used
    title: 'Daftar Todos',
    // all titles will be injected into this template
    titleTemplate: '%s | TODOSLIST'
  },
  components: {
    FooterPage,
    Navbar,
    HomePage
  },
  data () {
    return {
      HomePage: []
    }
  },
  created () {
    this.gettodos()
  },
  methods: {
    gettodos () {
      server
        .get('/activity-groups', {
        })
        .then(({ data }) => {
          this.HomePage = data
          console.log(data)
        })
        .catch((err) => {
          console.log(err)
        })
    }
  }
}
</script>

<style></style>
