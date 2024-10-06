<script setup>
import Card from "./Card.vue";

const onClickAdd = () => {};
const onClickFavorite = () => {};
</script>

<template>
    <div class="grid grid-cols-4 gap-10">
        <Card
            v-bind:image-url="'/sneakers/sneakers-1.jpg'"
            v-bind:title="'Мужские Кроссовки Nike Blazer Mid Suede'"
            v-bind:price="1205"
            v-bind:is-added="true"
            v-bind:is-favorite="true"
            v-bind:on-click-add="() => {}"
            v-bind:on-click-favorite="() => {}"
        />
    </div>
</template>

<style lang="scss" scoped></style>
