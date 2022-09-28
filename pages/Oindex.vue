<template>
  <!-- <v-card> -->
  <!--   <v-layout> -->
  <!--     <v-navigation-drawer expand-on-hover rail> -->
  <!--       <v-list> -->
  <!--         <v-list-item prepend-avatar="https://randomuser.me/api/portraits/men/85.jpg" title="João Adams" -->
  <!--           subtitle="jadams@gmailcom"></v-list-item> -->
  <!--       </v-list> -->

  <!--       <v-divider></v-divider> -->

  <!--       <v-list density="compact" nav> -->
  <!--         <v-list-item prepend-icon="mdi:mdi-folder" title="My Files" value="myfiles"></v-list-item> -->
  <!--         <v-list-item prepend-icon="mdi:mdi-account-multiple" title="Shared with me" value="shared"></v-list-item> -->
  <!--         <v-list-item prepend-icon="mdi:mdi-star" title="Starred" value="starred"></v-list-item> -->
  <!--       </v-list> -->
  <!--     </v-navigation-drawer> -->

  <!--     <v-main style="height: 350px"> -->
  <!--       <v-select v-model="select" :hint="`${select.state}, ${select.abbr}`" :items="items" item-title="state" -->
  <!--         item-value="abbr" label="Select" persistent-hint return-object single-line></v-select> -->
  <!--     </v-main> -->
  <!--   </v-layout> -->
  <!-- </v-card> -->
  <NuxtLayout>oi</NuxtLayout>
</template>

<script>
export default {
  name: "index.vue",

  data: () => ({
    drawer: false,
    group: null,
    items: [
      {
        title: 'Foo',
        value: 'foo',
      }],
    select: { state: 'Florida', abbr: 'FL' },
    items: [
      { state: 'Florida', abbr: 'FL' },
      { state: 'Georgia', abbr: 'GA' },
      { state: 'Nebraska', abbr: 'NE' },
      { state: 'California', abbr: 'CA' },
      { state: 'New York', abbr: 'NY' },
    ],
  }),

  watch: {
    group() {
      this.drawer = false
    },
  },
}
</script>
