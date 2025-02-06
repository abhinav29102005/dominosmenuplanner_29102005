# DOMINOS-MENU-PLANNER

Description
The Domino’s Meal Planner is a Jetpack Compose-based Android app that helps users select the best meal combinations within a specified budget. It allows users to enter their budget, browse potential meal combos, and get meal suggestions based on Domino's menu. The UI follows Domino's signature color scheme and branding.

⭐ Features

1️⃣ User Input for Budget
Users can enter their desired budget.

The app dynamically updates meal combinations based on the budget entered.

2️⃣ Dynamic Meal Combination Generator
Generates meal combos that fit within the specified budget.
Displays multiple meal options for a given budget.


3️⃣ Custom UI & Branding
Uses Domino’s official colors (Red, Blue, White).
Includes Domino’s logo for a visually appealing interface.


4️⃣ Menu Items & Pricing
Includes pizzas, sides, desserts, beverages, and meal combos.
Prices are stored in a List<MenuItem>.


5️⃣ Card-Based UI for Meal Display
Each meal combination is displayed in a separate card.
Includes:
List of selected items.
Total cost.
Domino's branding (logo, colors).


6️⃣ Uses Jetpack Compose
TextField for budget input.
LazyColumn to display meal combinations efficiently.
State management (remember) ensures the UI updates dynamically.



⚠️ Loopholes & Issues


❌ 1. Inefficient Combination Generation Algorithm
The calculateCombinations() function uses a nested loop approach.
It does not check all possible combinations, leading to incomplete meal options.
Better approach: Implement Backtracking or Dynamic Programming for optimal solutions.

❌ 2. No Handling for Edge Cases in Budget Input
If the user enters zero or a very low budget, the app may not return any combinations.
There is no minimum budget limit, leading to situations where no meals are found.

❌ 3. No Sorting or Prioritization of Meal Combinations
The app does not prioritize the best meal combos (e.g., best value-for-money).
Better approach: Sort combos based on total calories, popularity, or user preferences.

❌ 4. UI Scaling Issues for Larger Budgets
If a user enters a very high budget, the app may generate too many options, causing performance issues.
Better approach: Implement pagination or limit the number of displayed results.

❌ 5. No Error Handling for Non-Numeric Input
If the user enters letters or symbols instead of numbers, the app crashes.
Better approach: Use try-catch or isDigit() to validate input.

❌ 6. No Database or API Integration
The menu is hardcoded in the app.
Issue: If Domino’s changes their menu or prices, the app becomes outdated.
Better approach: Fetch menu data from an API or Firebase.

❌ 7. No Option to Filter or Customize Meals
Users cannot filter meals by:
Vegetarian vs. Non-Vegetarian
Calories / Health-conscious options
Specific ingredients (e.g., cheese, chicken)
Better approach: Add filter options for a better user experience.

✅ Potential Improvements

🚀 Implement a smarter combination-finding algorithm (e.g., Backtracking or Knapsack Problem).
📊 Sort results by value, taste, or popularity to give the best recommendations.
🔄 Fetch menu dynamically from an API instead of hardcoding it.
🔍 Allow users to filter meals based on preferences (Veg, Non-Veg, Calories).
🛠️ Improve UI performance for large budgets (pagination, lazy loading).



Final Verdict 🏆


✅ Great concept for a budget-based meal planner.
⚠️ Needs optimization in algorithm, UI performance, and error handling.
🚀 Adding API & filters would make it a game-changer!
