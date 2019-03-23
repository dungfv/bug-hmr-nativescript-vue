<template>
    <page>
        <stack-layout>
            <button text="go to page 2" @tap="goto()" class="btn btn-info"></button>
        </stack-layout>
    </page>
</template>
<script>
    import Page2 from './page2.vue'
    export default {
        methods: {
            goto() {
                this.$navigateTo(Page2)
            }
        }
    }
</script>