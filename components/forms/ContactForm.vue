<template>
  <v-container>
    <form name="contactPage" action="/thanks" method="POST" netlify netlify-honeypot>
      <p class="hidden">
        <label>
          Don’t fill this out if you’re human: <input name="bot-field" />
        </label>
      </p>
      <v-container>
        <v-row>
          <input type="hidden" name="form-name" value="contactPage" />
          <v-col
            cols="12"
            md="6">
            <v-text-field
              id="name"
              label="Your Name"
              type="text"
              required></v-text-field>
          </v-col>

          <v-col
            cols="12"
            md="6">
            <v-text-field
              id="email"
              label="E-mail"
              type="email"
              required></v-text-field>
          </v-col>
        </v-row>
        <v-row>
          <v-col>
            <v-textarea id="message" label="Message"></v-textarea>
          </v-col>
        </v-row>
        <v-btn
          class="me-4"
          type="submit">
          submit
        </v-btn>
      </v-container>
    </form>
  </v-container>
</template>

