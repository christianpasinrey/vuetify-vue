<script setup>
  import { ref,computed } from 'vue'

  const myData = ref({
    name: 'John Leider',
    email: 'john@email.net',
    phone: '555-555-5555',
    address: '1234 Main St',
    city: 'San Francisco',
    state: 'CA',
    zip: '94111',
  })
</script>
<template>
    <v-card
      variant="tonal"
      style="width:full-width;margin-top:50px"
      class="mx-auto"
    >
      <v-card-title>My Account</v-card-title>
      <v-card-text style="width:600px">
        <v-row style="width:600px">
          <v-col cols="12" md="6">
            <v-text-field
              label="Name"
              v-model="myData.name"
            ></v-text-field>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field
              label="Email"
              v-model="myData.email"
            ></v-text-field>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field
              label="Phone"
              v-model="myData.phone"
            ></v-text-field>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field
              label="Address"
              v-model="myData.address"
            ></v-text-field>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field
              label="City"
              v-model="myData.city"
            ></v-text-field>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field
              label="State"
              v-model="myData.state"
            ></v-text-field>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field
              label="Zip"
              v-model="myData.zip"
            ></v-text-field>
          </v-col>
        </v-row>
      </v-card-text>
      <v-card-actions>
        <v-spacer></v-spacer>
        <v-btn color="primary">Save</v-btn>
      </v-card-actions>
    </v-card>
</template>
