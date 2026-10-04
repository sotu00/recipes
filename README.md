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
