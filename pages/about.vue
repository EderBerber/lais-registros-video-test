<template>
    <v-card>
        <v-tabs v-model="tab" align-tabs="center">
            <v-tab :value="1">Proyecto</v-tab>
            <v-tab :value="2">Documentación</v-tab>
            <v-tab :value="3">Créditos</v-tab>
        </v-tabs>
        
        <v-window v-model="tab">
            <v-window-item v-for="n in 3" :key="n" :value="1" >
                <p>
                    Texto proyecto
                </p>
            </v-window-item>
            <v-window-item v-for="n in 3" :key="n" :value="2" >
                <p>
                    Doc texto
                </p>
            </v-window-item>
            <v-window-item v-for="n in 3" :key="n" :value="3" >
                <p>
                    Creditos texto
                </p>
            </v-window-item>
        </v-window>
    </v-card>
</template>

<script setup>
const tab = ref(null)
const text = ref('Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.')

</script>