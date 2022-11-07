<template>
    <div>
        <button @click="useMeChild" v-on="$listener">
            <slot></slot>
        </button>
    </div>
</template>

<script>
    export default {
        name: 'AppButton',
        methods: {
            useMeChild() {
                console.log("Clicked Use me from Child");
            }
        }
    }
</script>

<style lang="scss" scoped>
    button {
        color: white;
        background: green;
        font-size: 22px;
        border: none;
        appearance: none;
        margin: 20px;
        padding: 20px;
        &:hover {
            box-shadow: 0 0 0 10px green;
        }
    }
</style>