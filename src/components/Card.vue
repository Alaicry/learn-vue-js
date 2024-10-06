<script setup>
defineProps({
    imageUrl: String,
    title: String,
    price: Number,
    isFavorite: Boolean,
    isAdded: Boolean,
    onClickAdd: Function,
    onClickFavorite: Function,
});
</script>

<template>
    <div
        class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
    >
        <img
            v-bind:src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
            v-bind:alt="isFavorite ? 'like-2' : 'like-1'"
            v-on:click=""
            class="absolute top-8 left-8"
        />
        <img v-bind:src="imageUrl" alt="Sneaker" />
        <p class="mt-2">{{ title }}</p>
        <div class="flex justify-between mt-5">
            <div class="flex flex-col">
                <span class="text-slate-400">Цена :</span>
                <b>{{ price }} руб</b>
            </div>
            <img
                v-bind:src="isAdded ? '/checked.svg' : '/plus.svg'"
                v-bind:alt="isAdded ? 'checked' : 'plus'"
                v-on:click=""
            />
        </div>
    </div>
</template>

<style lang="scss" scoped></style>
