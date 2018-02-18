<template>
  <v-layout>
    <v-flex text-xs-center>
      <v-form v-model="valid">
        <v-text-field
          label="Name"
          v-model="name"
          :rules="nameRules"
          required
        ></v-text-field>
        <v-text-field
          label="E-mail"
          v-model="email"
          :rules="emailRules"
          required
        ></v-text-field>
        <v-btn
          @click="submit"
          :disabled="!valid"
        >Login</v-btn>

      </v-form>
    </v-flex>
  </v-layout>
</template>
