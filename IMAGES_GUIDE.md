# How to Add Images to Your Portfolio

This guide explains how to add your images to the portfolio website.

## Folder Structure

Create an `images` folder in your project root to organize your images:

```
Portfolio Madre/
├── images/
│   ├── banner/
│   │   └── banner-image.jpg
│   ├── gallery/
│   │   ├── artwork-1.jpg
│   │   ├── artwork-2.jpg
│   │   ├── artwork-3.jpg
│   │   └── ...
│   └── about/
│       └── artist-photo.jpg
├── index.html
├── about.html
└── ...
```

## 1. Adding the Banner Image (Homepage)

The banner image appears at the top of the homepage behind the artist name.

**Option A: Background Image (Recommended)**
- Edit `styles.css`
- Find the `.banner` class
- Add: `background-image: url('images/banner/banner-image.jpg');`
- Add: `background-size: cover;` and `background-position: center;`

**Option B: As an `<img>` tag**
- Edit `index.html`
- Add an `<img>` tag inside the `.banner` section

## 2. Adding Gallery Images (Homepage)

Replace the placeholder divs with `<img>` tags:

**In `index.html`, replace:**
```html
<div class="gallery-item">
    <div class="placeholder-image"></div>
</div>
```

**With:**
```html
<div class="gallery-item">
    <img src="images/gallery/artwork-1.jpg" alt="Artwork title" class="gallery-image">
</div>
```

Repeat for each gallery image.

## 3. Adding Artist Photo (About Page)

**In `about.html`, replace:**
```html
<div class="artist-photo"></div>
```

**With:**
```html
<img src="images/about/artist-photo.jpg" alt="Artist Name" class="artist-photo">
```

## Image Recommendations

- **Banner image:** 1920x1080px or larger, landscape orientation
- **Gallery images:** 800x800px to 1200x1200px (square works best, but any ratio is fine)
- **Artist photo:** 600x600px to 800x800px (square recommended)
- **Format:** JPG or PNG
- **Optimization:** Compress images before uploading for faster loading (use tools like TinyPNG, ImageOptim, or similar)

## Tips

- Use descriptive filenames (e.g., `sunset-painting-2024.jpg` instead of `IMG_1234.jpg`)
- Keep file sizes reasonable (aim for under 500KB per image)
- Use alt text for accessibility (describe what's in the image)

