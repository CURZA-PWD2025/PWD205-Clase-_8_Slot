<template>
    <button>

        <slot name="pre_icon"></slot>
        <slot name="texto_boton">Texto Default</slot>
        <slot name="post_icon"></slot>


    </button>
</template>
<style scoped>
button {
    background-color: #4CAF50;
    transition: 0.3s ease all;

    /* Green */
    &:hover {
        background-color: #3a893e;
    }
}
</style>