<template>
<section class="single-recipe">
    <h1>{{ $route.params.id }}</h1>
    <div>
        <img src="" alt="">
    </div>
    <p>the recipe description....</p>
</section>
</template>

<style>
    .single-recipe{
        display: center;
        flex-flow: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 30px;
    }
</style>
