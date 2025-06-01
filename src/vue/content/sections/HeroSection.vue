<template>
    <!-- Heading Section -->
    <PageHeader :id="props.id"
                title="*Кэмпинг* для всей семьи"
                subtitle="Успей арендовать <strong>кемпинг</strong> для себя и для своей <strong>семьи</strong>"
                label="и встречай рассвет у реки"
                logo-url="images/logo/camping-logo.png"
                :show-button="true"
                button-icon="fa-solid fa-search"
                button-label="Дальше"
                button-url="#about"/>
</template>

<script setup>
import PageHeader from "/src/vue/components/layout/PageHeader.vue"

const props = defineProps({
    id: String
})
</script>

<style lang="scss" scoped>
@import "/src/scss/_theming.scss";
</style>