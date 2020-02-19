<template>
    <v-app>
        <v-content class="bg">
            <v-row>
                <Keyaki />
                <Nogi />
                <Hinata />
            </v-row>
        </v-content>
    </v-app>
</template>

<style>
    .bg {
        background-size: cover;
        background-image: url("~@/assets/images/back_sakamichi.png");
    }
</style>

<script>
import Keyaki from '~/pages/keyaki'
import Nogi from '~/pages/nogi'
import Hinata from '~/pages/hinata'

export default {
    components: {
        Keyaki,
        Nogi,
        Hinata
    }
}
</script>
