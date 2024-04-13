<template>
    <v-app>
        <v-main>
            <login></login>
        </v-main>
    </v-app>
</template>

<script>
import Login from './components/Login.vue'

export default {
    name: 'App',

    components: {
        Login
    },

    data: () => ({
        //
    })
}
</script>
