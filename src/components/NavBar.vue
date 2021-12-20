<template>
    <div class="navbar">
        <div class="left">
            <div class="option">AMVD</div>
        </div>
        <div class="right">
            <div class="option">Log in</div>
            <div class="option">Sign in</div>
        </div>
    </div>
</template>

<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
    setup() {
        
    },
})
</script>

<style scoped>
    .navbar{
        width: 100%;
        background-color: rgb(23, 201, 100);
        position: fixed;
        top: 0;
        left: 0;
        display: flex;
        flex-direction: row;
    }
    .left{
        width: 50%;
        display: flex;
        flex-direction: row;
        justify-content: left;
    }
    .right{
        width: 50%;
        display: flex;
        flex-direction: row;
        justify-content: right;
    }
    .option{
        padding: 1rem 2rem;
        border-bottom: 3px solid transparent;
        background-color: rgb(23, 201, 100);
        transition: all ease 0.3s;
    }
    .option:hover{
        border-bottom: 3px solid rgb(199, 252, 222);
        background-color: rgb(45, 219, 121);
        cursor: pointer;
    }
</style>