<template>
  <section>
    <div id="form-add" class="container-add">
      <div class="row m-5 no-gutters shadow-lg">
        <div class="col-md-6 bg-white p-5">
          <h3 class="pb-3 text-center">ADD NEWS</h3>
          <div class="form-style">
            <form id="add-formbyNews">
              <div class="form-group pb-3">
                <input
                  type="text"
                  placeholder="Nama List Iteam"
                  class="form-control"
                  id="add-news"
                />
              </div>
              <div class="col-auto my-1">
                <select class="custom-select mr-sm-2" id="add-priotity">
                  <option value="null" selected>..Choose PRIORITY..</option>
                </select>
              </div>
              <br />
              <div class="pb-2">
                <button
                  type="submit"
                  class="btn btn-primary w-100 font-weight-bold mt-2 text-center"
                  id="submit"
                >
                  Submit
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
// import server from '@/api'
export default {
  name: 'AddNews',
  data () {
    return {
      title: '',
      priority: ''
    }
  },
  methods: {
    async submit () {
      this.$router.push('/home')
    }
  }
}
</script>

<style></style>
