<script>
import AppHeader from "./components/AppHeader.vue"
import AppContent from "./components/AppContent.vue"
import AppPagesNav from "./components/AppPagesNav.vue"
import AppFooter from "./components/AppFooter.vue"
import AppSocialFooter from "./components/AppSocialFooter.vue"

export default {
    components: {
        AppHeader,
        AppContent,
        AppPagesNav,
        AppFooter,
        AppSocialFooter
    }
}
</script>

<template>
    <AppHeader />
    <AppContent />
</template>

<style lang="scss"></style>