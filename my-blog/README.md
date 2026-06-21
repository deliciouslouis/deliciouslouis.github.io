# Blog



## Files in this folder

- `index.Rmd` — your homepage
- `about.Rmd` — your about page
- `posts/post1.Rmd` — example blog post (copy this for every new post)
- `_site.yml` — site settings (change the title here)

---

## How to build and publish

### Step 1 — Open in RStudio
Open any `.Rmd` file in RStudio.

### Step 2 — Build the site
In the RStudio console, run:
```r
rmarkdown::render_site()
```
This turns all your `.Rmd` files into `.html` files.

### Step 3 — Push to GitHub
Upload all the files (including the generated `.html` files) to a GitHub repository
named exactly: `yourusername.github.io`

### Step 4 — Enable GitHub Pages
- Go to your repo on GitHub
- Click Settings → Pages
- Set Source to "Deploy from a branch" → main → / (root)
- Hit Save

Your site will be live at `https://yourusername.github.io` in a minute or two!

---

## Adding a new blog post

1. Copy `posts/post1.Rmd` and rename it (e.g. `posts/my-new-post.Rmd`)
2. Edit the title and write your content
3. Add a link to it in `index.Rmd` like this:
   `[Post Title](posts/my-new-post.html)`
4. Run `rmarkdown::render_site()` again
5. Push to GitHub

---

## Changing the site name

Edit the `title:` line at the top of `index.Rmd` and the `title:` in `_site.yml`.
