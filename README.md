function calculateChaiIngredients() {
    // Prompt the user for the number of cups
    let numberOfCups = prompt("Karibu! How many cups of Chai Bora would you like to make?");
    
    // Convert the input to a number
    numberOfCups = Number(numberOfCups);

    // Check if the input is a valid number
    if (isNaN(numberOfCups) || numberOfCups <= 0) {
        console.log("Please enter a valid number of cups.");
        return;
    }

    // Calculate the required amount of each ingredient
    const water = 200 * numberOfCups; // 200 ml per cup
    const milk = 50 * numberOfCups; // 50 ml per cup
    const teaLeaves = 1 * numberOfCups; // 1 tablespoon per cup
    const sugar = 2 * numberOfCups; // 2 teaspoons per cup

    // Print the results
    console.log(`To make ${numberOfCups} cups of Kenyan Chai, you will need:`);
    console.log(`Water: ${water} ml`);
    console.log(`Milk: ${milk} ml`);
    console.log(`Tea Leaves (Majani): ${teaLeaves} tablespoons`);
    console.log(`Sugar (Sukari): ${sugar} teaspoons`);
    console.log("\nEnjoy your Chai Bora!");
}

// Call the function to test it
calculateChaiIngredients();
