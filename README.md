# Blog

Personal blog hosted on GitHub Pages.

**Live site:** https://bowensu123.github.io/blog/

## Structure

```
blog/
├── index.html              # Homepage (post list)
└── posts/
    └── <slug>/
        ├── index.html      # Post content
        └── assets/         # Post-specific assets (css, js, images)
```

Each post lives in its own directory under `posts/`, with its own self-contained
assets. Adding a new post = create a new folder + add an entry to `index.html`.

## Add a new post

1. Create a new directory: `posts/<your-slug>/`
2. Put your article HTML at `posts/<your-slug>/index.html`
3. Put any images/CSS/JS in `posts/<your-slug>/assets/`
4. Add a new `<li>` to the post list in the root `index.html`
5. Commit & push:

```bash
git add .
git commit -m "Add post: <title>"
git push
```


## Local preview

```bash
python -m http.server 8000
```

Then open http://localhost:8000
