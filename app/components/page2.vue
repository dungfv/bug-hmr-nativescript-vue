<template>
    <page>
        <stack-layout>
            <button text="go to page 3" class="btn btn-info" @tap="goto()"></button>
        </stack-layout>
    </page>
</template>
<script>
    import Page3 from './page3.vue'
    export default {
        methods: {
            goto() {
                this.$navigateTo(Page3)
            }
        }
    }
</script>