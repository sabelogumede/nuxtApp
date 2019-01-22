<template>
    <section class="recipes">

        <!-- recipe loop through recipes-->
        <Recipe
        
            v-for="recipe in recipes"
            :key="recipe.id"
            :thumbnail="recipe.thumbnail" 
            :title="recipe.title"
            :previewText="recipe.previewText"
            :id="recipe.id" 
            />

    </section>
</template>

// registering our recipe import component
<script>
import Recipe from '@/components/Recipe'
import { setTimeout } from 'timers';

export default {
    components: {
        Recipe
    },
    asyncData() {
        return new Promise((resolve, reject) =>{
            setTimeout(() => {
                resolve({
                    recipes: [
                        {
                            id:"1",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            thumbnail: "https://www.primaverakitchen.com/wp-content/uploads/2018/12/Low-Carb-Shrimp-Fajita-Meal-Prep-Bowls-Primavera-Kitchen-3-500x660.jpg"
                        },
                        {
                            id:"2",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            thumbnail: "http://images.media-allrecipes.com/images/74681.jpg"
                        },
                        {
                            id:"3",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            thumbnail: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQqXknXshTE2WXMoy6KhmRRlqg0Oeet0Y9Ao6onD-HdoH0AL7qLA"
                        },
                        {
                            id:"4",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            thumbnail: "https://www.primaverakitchen.com/wp-content/uploads/2018/12/Low-Carb-Shrimp-Fajita-Meal-Prep-Bowls-Primavera-Kitchen-3-500x660.jpg"
                        }
                    ]
                })
            }, 1500)
        })
    }
};

</script>

// css
<style scoped>
    .recipes {
        display: flex;
        flex-flow: row wrap;
        justify-content: center;
        align-items: center;
    };

</style>
