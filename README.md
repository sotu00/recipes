# Split-Protein Dinners

Six static recipe pages with schema.org Recipe markup (JSON-LD plus microdata), built so AnyList's recipe importer can read them.

## Publish with GitHub Pages

1. Create a public repository (for example `recipes`) and commit every file in this folder to the root of `main`.
2. In the repository, go to Settings, then Pages. Set the source to "Deploy from a branch", branch `main`, folder `/ (root)`.
3. After a minute the site is live at `https://<username>.github.io/recipes/`.

With the GitHub CLI:

```
gh repo create recipes --public --source=. --push
gh api -X POST repos/{owner}/recipes/pages -f "source[branch]=main" -f "source[path]=/"
```

## Import into AnyList

Open one recipe page at a time (not the index) and use the AnyList browser extension or the AnyList Recipe Import share action.

## Adding a recipe

Copy any recipe page, then edit both the JSON-LD block in the head and the visible HTML so they match.

## Photo credits

The photos are representative stock images from Unsplash, used under the [Unsplash License](https://unsplash.com/license). They are not photos of these exact recipes.

- `thai-red-curry.jpg`: [Alyssa Kowalski](https://unsplash.com/photos/bowl-of-food-97YFGmT3Cu8)
- `sheet-pan-fajitas.jpg`: [Thomas Park](https://unsplash.com/photos/a-wooden-table-topped-with-plates-of-food-G3hZMCdLUdw)
- `egg-roll-in-a-bowl.jpg`: [Mario Raj](https://unsplash.com/photos/vegetable-salad-on-white-ceramic-plate-UhwdAcjk_zo)
- `greek-bowls.jpg`: [amin ramezani](https://unsplash.com/photos/a-bowl-of-salad-PipzrGSil-c)
- `bunless-burgers.jpg`: [You Le](https://unsplash.com/photos/a-plate-of-food-SSOQvW4Am2k)
- `two-pot-chili.jpg`: [Svitlana](https://unsplash.com/photos/a-bowl-of-food-VAbBclifmvY)
