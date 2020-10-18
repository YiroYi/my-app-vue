<template>
  <li>
    <h2>{{ friend.name }}</h2>
    <button @click="toggleDetails">{{ detailsAreVisible ? 'Hide' : 'Show' }} Details</button>
    <ul v-if="detailsAreVisible">
      <li><strong>Phone: {{ friend.phone }} </strong></li>
      <li><strong>Email: {{ friend.mail }}</strong></li>
    </ul>
  </li>
</template>

<script>
  export default {
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
