<script setup>
import Card from "./components/Card.vue";
import CardList from "./components/CardList.vue";
import Header from "./components/Header.vue";
import Container from "./UI/Container.vue";
import Main from "./UI/Main.vue";
</script>

<template>
    <Container>
        <Header />
        <Main>
            <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>
            <CardList />
        </Main>
    </Container>
</template>

<style scoped></style>
