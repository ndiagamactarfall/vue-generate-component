<template lang="{{filesType.html}}">
{% if filesType.html === 'jade' || filesType.html === 'pug' %}
  section(class="{{name | kebabCase}}")
    h1 {{name | kebabCase}} Component
{% else %}
  <section class="{{name | kebabCase}}">
    <h1>{{name | kebabCase}} Component</h1>
  </section>
{% endif %}
</template>

<script lang="{{ filesType.js }}">
  export default  {
    name: '{{name | kebabCase}}',
    props: [],
    mounted() {

    },
    data() {
      return {

      }
    },
    methods: {

    },
    computed: {

    }
}
</script>

<style scoped lang="{{ filesType.style }}">
  .{{name | kebabCase}} {

  }
</style>
