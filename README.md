# 🍽️ Smart Recipe Generator

The **Smart Recipe Generator** is a command-line Python tool that helps you discover delicious recipes based on the ingredients you have at home. You can filter recipes by dietary preferences (e.g., vegetarian, keto) and preparation time, then save your favorite results in CSV or TXT formats.

---

## 📸 Preview

```bash

🍽️  Welcome to the Smart Recipe Generator!
Enter at least 5 ingredients (comma-separated): onion, chilli, garlic, potato, egg, tomato

Select a dietary preference:
1. none
2. vegetarian
3. vegan
4. gluten free
5. ketogenic
6. pescetarian
7. paleo
Choose an option (1-7): 1
Maximum prep time in minutes (or press Enter to skip): 30

🔍 Searching recipes...

🧾 Top Recipes:

1. Spanish Omelette
   🕒 25 minutes | 👨‍🍳 2 servings
   🔗 https://spoonacular.com/spanish-omelette-123456
   🥕  Used ingredients: potato, egg, onion
   🚫  Missing ingredients: olive oil, salt
   Recipe ID: 123456

2. Spicy Garlic Potato Stir Fry
   🕒 20 minutes | 👨‍🍳 3 servings
   🔗 https://spoonacular.com/spicy-garlic-potato-stir-fry-789012
   🥕  Used ingredients: garlic, potato, chilli
   🚫  Missing ingredients: soy sauce, spring onion
   Recipe ID: 789012

3. Tomato Egg Curry
   🕒 30 minutes | 👨‍🍳 4 servings
   🔗 https://spoonacular.com/tomato-egg-curry-345678
   🥕  Used ingredients: egg, tomato, garlic
   🚫  Missing ingredients: curry leaves, mustard seeds
   Recipe ID: 345678

💾 Choose file format to save:
0. Skip saving
1. CSV (.csv)
2. Text File (.txt)
Your choice: 1
Enter filename (without extension): my_recipes
✅ Recipes saved to 'my_recipes.csv'.


```
---

## 🚀 How to Run

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/smart-recipe-generator.git
   cd smart-recipe-generator
   ```

2. **Install dependencies**
   Use `pip` to install the required Python libraries.

   ```bash
   pip install requests
   ```

3. **Get your Spoonacular API Key**

   * Visit [Spoonacular](https://spoonacular.com/food-api) and sign up for a free account.
   * Copy your **API key** from the dashboard.

4. **Add your API key**
   Replace the placeholder in the script:

   ```python
   API_KEY = "*******************************"
   ```

5. **Run the script**

   ```bash
   python recipe_generator.py
   ```

---

## 🧰 Libraries Used

| Library    | Description                         | Installation Command   |
| ---------- | ----------------------------------- | ---------------------- |
| `requests` | For making HTTP requests to the API | `pip install requests` |
| `csv`      | For saving results to a `.csv` file | *(built-in module)*    |

---

## 🧠 Features

* ✅ Input at least **5 ingredients** to get started.
* ✅ Filter recipes by:

  * 🥦 Dietary preference (e.g., vegan, paleo)
  * ⏱️ Maximum prep time
* ✅ View top 5 recipe suggestions with:

  * Preparation time
  * Servings
  * Direct link to the recipe
  * Used & missing ingredients
* ✅ Export results to:

  * CSV (`.csv`)
  * Text file (`.txt`)

---

## 🔐 Notes

* Ensure you keep your **API key private**. Do not upload it to public repositories.
* If you hit usage limits, try again after a while or consider upgrading your API plan on Spoonacular.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Support

If you find a bug or want to contribute, feel free to open an issue or submit a pull request!

---
