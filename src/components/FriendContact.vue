<template>
  <li>
    <h2>{{ name }}</h2>
    <button @click="toggleDetails">{{ detailsAreVisible ? 'Hide' : 'Show' }} Details</button>
    <ul v-if="detailsAreVisible">
      <li><strong>Phone: {{ phoneNumber }} </strong></li>
      <li><strong>Email: {{ emailAddress }}</strong></li>
    </ul>
  </li>
</template>

<script>
  export default {
    props: [
      'name',
      'phoneNumber',
      'emailAddress'
    ],
    data() {
      return {
        detailsAreVisible: false,
        friend: {
          id: 'Kripto',
          name: "Kripto Yi",
          phone: '434322',
          mail: 'kripto@test.com'
        }
      }
    },
    methods: {
      toggleDetails() {
        this.detailsAreVisible = !this.detailsAreVisible
      }
    }
  };
</script>
