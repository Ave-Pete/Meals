# Recipe Suggester

The user has told you they have certain ingredients. Your job is to suggest the best matching recipe(s) from their collection.

## Instructions

1. Read all the recipe `.md` files in the current directory (ignore `README.md`, `INDEX.md`, `CUPBOARD.md`).
2. The user's ingredients are: **$ARGUMENTS**
3. For each recipe, check whether the user's ingredients cover the main components (i.e. the protein, veg, or key flavour base). Ignore staple cupboard items — spices, oil, flour, sugar, salt, garlic, eggs — when deciding if there's a match. Focus on the hero ingredients.
4. Rank the recipes by how well they match. A recipe where the user has the main ingredient(s) ranks highest.
5. Suggest the **top 1–3 matches** only. For each, give:
   - Recipe name (as a markdown link to the file)
   - One sentence on why it matches their ingredients
   - Any key missing ingredients they'd need to buy
6. If nothing matches well, say so honestly and suggest the closest option with what they'd need to pick up.

Keep the response concise — this is a quick "what should I cook tonight?" helper, not a full recipe printout.
