<script setup>
import { RouterLink } from 'vue-router';
</script>

<template>
    <header>
        <nav class="container">
            <div class="branding">
                <img src="../assets/todo.png" alt="logo">
                <h1>TodoList</h1>
            </div>
            <ul class="nav-routes">
                <RouterLink to="/">
                    Home
                </RouterLink>
                <RouterLink to="/about">
                    About
                </RouterLink>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header {
    background-color: #f1f1f1;

    nav {
        display: flex;
        align-items: center;
        padding: 25px 16px;

        .branding {
            display: flex;
            align-items: center;
            gap: 8px;

            img {
                max-width: 50px;
                margin-top: -6px;
            }

            h1 {
                font-size: 18px;
            }
        }

        .nav-routes {
            display: flex;
            flex: 1;
            justify-content: flex-end;
            gap: 12px;
            list-style: none;

            a {
                text-decoration: none;
                color: inherit;
                font-size: 14px;
            }
        }
    }
}
</style>