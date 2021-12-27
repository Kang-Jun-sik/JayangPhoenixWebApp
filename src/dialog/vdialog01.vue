<template>
  <v-dialog
      v-model="dialog3"
      max-width="300"
  >
    <v-card>
      <v-card-title>
        Are you sure?

        <v-spacer/>

        <v-icon
            aria-label="Close"
            @click="dialog3 = false"
        >
          mdi-close
        </v-icon>
      </v-card-title>

      <v-card-text class="pb-6 pt-12 text-center">
        <v-btn
            class="mr-3"
            text
            @click="dialog3 = false"
        >
          Nevermind
        </v-btn>

        <v-btn
            color="success"
            text
            @click="dialog3 = false"
        >
          Yes
        </v-btn>
      </v-card-text>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  name: "vdialog01",
  data: () => ({
    dialog3: false
  })
}
</script>

<style scoped>

</style>
