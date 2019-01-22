<template>
    <head>
        <nav>
            <ul>
                <li><nuxt-link to="/">Staring Page</nuxt-link></li>
                <li><nuxt-link to="/recipes">Recipes</nuxt-link></li>
                <li><nuxt-link to="/about">About</nuxt-link></li>
            </ul>
        </nav>
    </head>
</template>

<style scoped>
    head {
        width: 100%;
        height: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #521751;
    }

    ul {
        list-style: none;
        padding: 0;
        margin: 0;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    li {
        margin: 0 10px;
    }
    a {
        text-decoration: none;
        color:white;
    }

</style>
