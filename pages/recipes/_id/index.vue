<template>
<section class="single-recipe">
    <h1>{{ recipe.title}}</h1>
    <div>
        <img class="recipe-image" :src="recipe.thumbnail" :alt="recipe.title">
    </div>
    <p>{{ recipe.descriptionText }}</p>
</section>
</template>

<script>
export default {
    asyncData(context) {
        return new Promise((resolve, reject) =>{
            setTimeout(() => {
                resolve({
                    recipe: [
                        {
                            id:"1",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            descriptionText: "this is a really delicious meal",
                            thumbnail: "https://www.primaverakitchen.com/wp-content/uploads/2018/12/Low-Carb-Shrimp-Fajita-Meal-Prep-Bowls-Primavera-Kitchen-3-500x660.jpg"
                        },
                        {
                            id:"2",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            descriptionText: "this is a really delicious meal",
                            thumbnail: "http://images.media-allrecipes.com/images/74681.jpg"
                        },
                        {
                            id:"3",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            descriptionText: "this is a really delicious meal",
                            thumbnail: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQqXknXshTE2WXMoy6KhmRRlqg0Oeet0Y9Ao6onD-HdoH0AL7qLA"
                        },
                        {
                            id:"4",
                            title: "Delicious Pizza",
                            previewText: "This is a descriptive text area",
                            descriptionText: "this is a really delicious meal",
                            thumbnail: "https://www.primaverakitchen.com/wp-content/uploads/2018/12/Low-Carb-Shrimp-Fajita-Meal-Prep-Bowls-Primavera-Kitchen-3-500x660.jpg"
                        }
                    ].find(el =>el.id === context.params.id)
                })
            }, 1500)
        })
    }
}
</script>




<style>
    .single-recipe{
        display: center;
        flex-flow: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 30px;
    }

    .recipe-image {
        width: 50%;
        height: 50%;
    }

</style>
