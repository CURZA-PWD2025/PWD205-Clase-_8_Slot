<template>
    <header>
        <div class="logo">
            <slot name="logo"></slot>
        </div>
        <nav>
            <slot name="menu-nav"></slot>
        </nav>
    </header>
    <main>
        <section>
            <slot name="main"></slot>
        </section>
        <aside>
            <slot name="aside"></slot>
        </aside>
    </main>
    <footer>
        <slot name="footer"></slot>
    </footer>

</template>

<script setup>

</script>

<style scoped>
header {
    padding: 1.25rem;
    width: 100%;
    background-color: #333;
    color: white;
    display: flex;
    justify-content: space-between;
}

main {
    position: relative;
    display: flex;
    justify-content: space-between;
    height: calc(100vh - 100px - 40px);
}

section {
    position: absolute;
    top: 0;
    left: 200px;
    width: 70%;
    padding: 20px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: calc(100vh - 100px - 40px);
}

aside {
    position: absolute;
    top: 0;
    left: 0;
    height: calc(100vh - 100px - 40px);
    width: 25%;
    padding: 20px;
    background-color: #474646;
}

footer {
    width: 100%;
    height: 40px;
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
    position: absolute;
    left: 0;
    bottom: 0px;
}
</style>