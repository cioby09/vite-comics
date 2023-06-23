<script>
import AppHeader from "./components/AppHeader.vue"
import AppContent from "./components/AppContent.vue"
import AppSubpages from "./components/AppSubpages.vue"
import AppFooter from "./components/AppFooter.vue"
import AppSocialFooter from "./components/AppSocialFooter.vue"

export default {
    components: {
        AppHeader,
        AppContent,
        AppSubpages,
        AppFooter,
        AppSocialFooter
    }
}
</script>

<template>
    <AppHeader />
    <AppContent />
    <AppSubpages />
    <AppFooter />
    <AppSocialFooter />
</template>

<style lang="scss"></style>