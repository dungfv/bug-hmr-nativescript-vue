<template>
    <Page>
        <ActionBar title="Welcome to NativeScript-Vue!"/>
        <GridLayout columns="*, auto" rows="*">
            <Label class="message" :text="msg" col="0" row="0"/>
            <button text="go to page 1" @tap="goto" class="btn btn-primary"></button>
        </GridLayout>
    </Page>
</template>

<script >
  import Page1 from './page1.vue'
  export default {
    data() {
      return {
        msg: 'Hello World!'
      }
    },
    methods: {
      goto() {
        this.$navigateTo(Page1)
      }
    }
  }
</script>

<style scoped>
    ActionBar {
        background-color: #53ba82;
        color: #ffffff;
    }

    .message {
        vertical-align: center;
        text-align: center;
        font-size: 20;
        color: #333333;
    }
</style>
