<template>
  <v-container fluid>
    <v-row align="center">
      <v-col class="d-flex" md="6" offset-md="3">
        <v-select :items="items" label="Escolha um produto."></v-select>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    items: ['Foo', 'Bar', 'Fizz', 'Buzz'],
  }),
}
</script>
