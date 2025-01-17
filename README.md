# WILCBOUW

Simple static _HTML_ website for the **WILCBOUW** organization.

## Development

The site is deployed to _GitHub Pages_ built from the `gh-pages` branch. For now
the proces is trigered manually or push changes to the `main` branch.

To deploy the site manually, first add your changes to the code and then add
them to the repository like this:

```sh
git add website/style.css
git commit -m "feat: Add animation style"
```

Then push the changes to the repository, but you need to use `git subtree`
option and the `--prefix` flag, it will look like this:

```sh
git subtree push --prefix website origin gh-pages
```

Then push the changes to the main branch of the repository:

```sh
git push origin main
```

To check the site locally, you can use this command in the terminal:

```sh
cd website
python3 -m http.server 8080
```

Then open a browser at this [localhost](http://localhost:8080/) address.
