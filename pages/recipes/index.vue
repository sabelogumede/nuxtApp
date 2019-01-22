<template>
    <section class="recipes">

        <!-- first recipe -->
        <Recipe 
            thumbnail="https://food.fnr.sndimg.com/content/dam/images/food/fullset/2014/2/19/1/FN_gluten-free-mac-n-cheese_s4x3.jpg.rend.hgtvcom.616.462.suffix/1393442138933.jpeg" 
            title="Delicious"
            previewText="this is a descriptive text area" />

        <!-- second recipe -->
        <Recipe 
            thumbnail="http://images.media-allrecipes.com/images/74681.jpg" 
            title="Delicious"
            previewText="this is a descriptive text area" />

        <!-- third recipe -->
        <Recipe 
            thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQqXknXshTE2WXMoy6KhmRRlqg0Oeet0Y9Ao6onD-HdoH0AL7qLA" 
            title="Delicious"
            previewText="this is a descriptive text area" />

        <!-- forth recipe -->
        <Recipe 
            thumbnail="https://www.primaverakitchen.com/wp-content/uploads/2018/12/Low-Carb-Shrimp-Fajita-Meal-Prep-Bowls-Primavera-Kitchen-3-500x660.jpg" 
            title="Delicious"
            previewText="This is a descriptive text area" />

    </section>
</template>

// js
// registering our recipe import component
<script>
import Recipe from '@/components/Recipe'

export default {
    components: {
        Recipe
    } 
}

</script>

// css
<style scoped>
    .recipes {
        display: flex;
        flex-flow: row wrap;
        justify-content: center;
        align-items: center;
    }

</style>
