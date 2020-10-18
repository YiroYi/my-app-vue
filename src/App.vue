<template>
  <section>
    <h2>Hello my friends</h2>
    <ul>
      <friend-contact></friend-contact>
      <friend-contact></friend-contact>
    </ul>
  </section>
</template>

<script>

export default {
  data() {
    return {
      friends: [
        {
          id: 'Kripto',
          name: "Kripto Yi",
          phone: '434322',
          mail: 'kripto@test.com'
        },
        {
          id: "Baily",
          name: "Baily Cobra",
          phone: '434322',
          mail: 'baily@test.com'
        }
      ]
    }
  }
}

</script>
