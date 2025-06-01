# smart_recipe_generator
This Python script is a Smart Recipe Generator that uses the Spoonacular API to suggest recipes based on user-provided ingredients and optional dietary preferences or time constraints.

✅ Key Features:
Ingredient Input:

Asks the user to input at least 5 ingredients.

Cleans and validates the input list.

Dietary Filters & Time Limit:

Offers a list of dietary preferences such as vegetarian, vegan, keto, etc.

Accepts a maximum preparation time (in minutes) as an optional filter.

Recipe Fetching:

Uses https://api.spoonacular.com/recipes/findByIngredients to fetch matching recipes (up to 10).

Fetches detailed info for each recipe using https://api.spoonacular.com/recipes/{id}/information.

Filtering & Display:

Filters recipes based on dietary preference and prep time.

Displays up to 5 top-matching recipes, including:

Title

Preparation time

Number of servings

Source URL

Used and missing ingredients

Save Options:

Offers option to save the results to:

.csv file (tabular format)

.txt file (formatted for readability)

🧠 How It Works (Internally):
User Input:
get_user_ingredients() and get_user_filters() gather user preferences.

API Calls:

fetch_recipe_ids() returns basic recipe matches based on ingredients.

fetch_recipe_details() fetches additional details like diet labels, time, URL, etc.

Filtering:
display_recipes() checks each recipe against optional filters and prints results.

Saving:
ask_save_format() calls save_to_csv() or save_to_txt() depending on the user's choice.

🔒 Notes:
You must replace the API key with a valid one from Spoonacular.

The script uses synchronous requests which could be slow if the API response time is high.

For production, error handling could be expanded to manage API limits and timeouts more gracefully.
