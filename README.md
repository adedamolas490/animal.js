// 1. Create the Body Parts first
addIngredient("animal_thigh", {
    type: "meat",
    color: "#d1a28a",
    shape: "drumstick",
    keywords: "meat,leg"
});

addIngredient("animal_ribs", {
    type: "meat",
    color: "#8a3324",
    shape: "ribs",
    keywords: "meat,bone"
});

// 2. Create the "Live" Animal
addIngredient("live_pig", {
    type: "meat",
    color: "#ffc0cb", // Pink
    shape: "bean_l", // Large bean shape for body
    keywords: "alive,animal,pig"
});

// 3. Create the "Butchering" Recipes
// This turns the pig into parts when combined with a knife
addRecipe("live_pig+knife", "animal_thigh");
addRecipe("live_pig+axe", "animal_ribs");

