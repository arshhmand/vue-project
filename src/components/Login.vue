<template>
    <v-container fluid fill-height>
        <v-layout class="ml-10">
            <v-card>
                <v-toolbar color="primary" :dark="true">
                    <v-toolbar-title>Login</v-toolbar-title>
                </v-toolbar>

                <v-card-text>
                    <v-form>
                        <v-text-field
                            prepend-icon="person"
                            type="text"
                            v-model="user.email"
                            label="E-mail"
                        />
                        <v-text-field
                            prepend-icon="lock"
                            type="password"
                            v-model="user.password"
                            label="Password"
                        />
                    </v-form>

                    <v-alert type="error" v-if="errorLogin"> Invalid Password or Email Id </v-alert>
                </v-card-text>

                <v-card-actions>
                    <div class="flex-grow-1"></div>
                    <v-btn color="primary" @click="login">Login</v-btn>
                </v-card-actions>
            </v-card>
        </v-layout>
    </v-container>
</template>
<script>
// import { AUTH_REQUEST } from '@/js/store/types/auth'
export default {
    name: 'login',
    data() {
        return {
            errorLogin: false,
            user: {}
        }
    },
    methods: {
        login() {
            // this.errorLogin = false
            // this.$store
            //     .dispatch(`auth/${AUTH_REQUEST}`, this.user)
            //     .then(() => {
            //         this.$router.push('/')
            //     })
            //     .catch(() => {
            //         this.errorLogin = true
            //     })
            // this.loading = false
            console.log('Hello')
        }
    }
}
</script>
