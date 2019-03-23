<template>
    <page>
        <stack-layout>
            <button text="go to page 4" class="btn btn-primary"></button>
            <button text="Home" @tap="home" class="btn btn-default"></button>
        </stack-layout>
    </page>
</template>
<script>
    import Home from './App.vue'
    export default {
        methods: {
            home() {
                this.$navigateTo(Home, {
                    clearHistory: true
                })
            }
        }
    }
</script>