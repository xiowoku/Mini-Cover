<template>
    <header>
        <div class="title-container">
            <h1>{{ title }}</h1>
        </div>
    </header>
</template>

<script>
export default {
    data() {
        return {
            title: import.meta.env.VITE_APP_TITLE
        };
    }
};
</script>

<style scoped>
header {
    display: flex;
    justify-content: center;
}

.title-container {
    display: flex;
    align-items: center;
    gap: 0.5rem;
}

.github-link {
    color: #666;
    transition: color 0.3s ease;
    display: flex;
    align-items: center;
}

.github-link:hover {
    color: #333;
}
</style>