<template>
    <div class="container-fluid bg-primary px-0 px-md-5">
        <div class="container pt-5 pb-5">
            <div class="row align-items-center px-3">
                <div class="col-lg-6 text-center text-lg-left">
                    <h1 class="display-3 font-weight-bold text-white">
                       TODO LIST
                    </h1>
                    <p class="text-white mb-4">
                        Buat Aktivity Pertama Mu.
                    </p>
                    <a href="/todo-items" class="btn btn-warning mt-1 py-3 px-5">Add News</a>
                </div>
                <div class="col-lg-6 text-center text-lg-right mb-n5">
                    <img class="img-fluid mt-5" src="../assets/images/sasa.png" alt="" />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HeroesSection',
  props: ['data']
}
</script>

<style>
</style>
