
<template>
   <div>
      <v-card class="mx-auto pa-12 pb-8" elevation="8" max-width="448" rounded="lg">
         <h5 class="mb-4">Sign in</h5>

         <v-text-field density="compact" placeholder="Email address" prepend-inner-icon="mdi-email-outline"
            variant="outlined"></v-text-field>

         <!-- <div class="text-subtitle-1 text-medium-emphasis d-flex align-center justify-space-between">
            Password

            <a class="text-caption text-decoration-none text-blue" href="#" rel="noopener noreferrer"
               target="_blank">
               Forgot login password?</a>
         </div> -->

         <v-text-field :append-inner-icon="visible ? 'mdi-eye-off' : 'mdi-eye'"
            :type="visible ? 'text' : 'password'" density="compact" placeholder="Enter your password"
            prepend-inner-icon="mdi-lock-outline" variant="outlined"
            @click:append-inner="visible = !visible"></v-text-field>

         <v-btn class="mb-8" color="blue" size="large" variant="tonal" block>
            Log In
         </v-btn>

         <v-card-text class="text-center">
            <h6 class="text-blue text-decoration-none">
               Sign up now <v-icon icon="mdi-chevron-right"></v-icon>
            </h6>
         </v-card-text>
      </v-card>
   </div>
</template>

<script>
export default {
   data: () => ({
      visible: false,
   })
}
</script>

<style scoped>

</style>