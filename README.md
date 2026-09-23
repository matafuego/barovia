# Curse of Strahd — comic site

## Folder structure
```
barovia-comic/
├── index.html
└── images/
    └── story/       ← carousel images for "The Story"
        ├── 01.jpg
        ├── 02.jpg
        ├── 03.jpg
        └── 04.jpg
```

## Adding more story images
1. Drop the new image file into `images/story/` (jpg or png).
2. Open `index.html`, find the `var slides = [...]` array near the bottom.
3. Add a new entry like:
   ```js
   {
     title: "No. 5",
     body: "Your caption here",
     img: "images/story/05.jpg"
   }
   ```
4. Save — no other changes needed.

As the diary, bestiary, and epilogue sections gain real art, the same
pattern applies: put images in a matching subfolder under `images/`
and reference them by relative path.

## Hosting
Upload this whole folder (keeping the structure intact) to any static
host — GitHub Pages, Cloudflare Pages, or Netlify all work by
dragging the folder in or connecting a repo. Then point your custom
domain at the host per its instructions.
