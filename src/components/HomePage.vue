<template>
  <section>
    <div>
      <b-card-group deck>
        <b-card>
          <b-card-text>
           {{ data.title }}
          </b-card-text>
          <template #footer>
            <small class="text-muted">{{ data.updated_at }}</small>
             <a
            class="btn btn-danger px-4"
            href="/activity-groups"
            role="button"
            >Delete</a
          >
          </template>
        </b-card>
      </b-card-group>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HomePage',
  props: ['data']
}
</script>

<style></style>
