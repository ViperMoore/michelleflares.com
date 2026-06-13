# Michelle Flares — Blog Files
## Deployment & Image Guide

---

## Files in this folder

```
blog/
├── blog.css                              ← Shared styles for ALL pages
├── index.html                            ← Blog listing page
├── does-my-business-need-a-website.html  ← Article 1
├── google-maps-beginners-guide.html      ← Article 2
├── ai-search-local-businesses.html       ← Article 3
└── images/                               ← PUT ALL IMAGES HERE
    ├── hero-need-website.jpg
    ├── hero-google-maps.jpg
    ├── hero-ai-search.jpg
    ├── inline-laptop-evening.jpg
    ├── inline-google-review.jpg
    └── inline-voice-assistant.jpg
```

---

## Step 1 — Add a Blog link to your main site nav

In your main `index.html`, find your nav links and add:
```html
<a href="/blog/">Blog</a>
```

---

## Step 2 — Generate images in Adobe Firefly

Export all images as **JPEG at 85% quality**.

### Hero images (1200 × 630px each)

**images/hero-need-website.jpg**
> "A friendly UK tradesperson — plumber or electrician — glancing at their phone on a job site, warm natural light, editorial documentary style, shallow depth of field, no text overlay, no logos"

**images/hero-google-maps.jpg**
> "Aerial perspective of colourful location map pins floating above a British high street, abstract and graphic, clean navy and warm amber colour palette, soft drop shadows, no text, no logos"

**images/hero-ai-search.jpg**
> "Abstract glowing digital network with soft light trails connecting small British shop storefronts, dark navy background, warm amber and soft purple glow, cinematic wide angle, no text, no logos"

### Inline images (1200 × 800px each)

**images/inline-laptop-evening.jpg**
> "A laptop open on a clean, minimal business website sitting on a kitchen table in the evening, warm lamp light, shallow depth of field, photorealistic, no text on screen"

**images/inline-google-review.jpg**
> "Close-up of hands holding a smartphone showing a five-star Google review screen, neutral light grey background, photorealistic, clean and modern"

**images/inline-voice-assistant.jpg**
> "A modern voice assistant smart speaker device sitting on a kitchen counter next to a person about to make a phone call, warm natural morning light, photorealistic, no brand logos visible"

---

## Step 3 — Replace placeholders with real images

Each placeholder has an HTML comment above it explaining exactly what to do.
Find the comment that starts with `<!-- HERO IMAGE INSTRUCTIONS` or `<!-- INLINE IMAGE INSTRUCTIONS`
and follow the swap instructions — it's just replacing a `<div>` with an `<img>` tag.

---

## Step 4 — Upload to GitHub

Push the entire `blog/` folder to the root of your repo.
Your URLs will be:
- michelleflares.com/blog/
- michelleflares.com/blog/does-my-business-need-a-website.html
- michelleflares.com/blog/google-maps-beginners-guide.html
- michelleflares.com/blog/ai-search-local-businesses.html

---

## Notes

- All internal links use absolute paths (`/blog/`, `/#contact`) so they work from any page depth.
- The shared `blog.css` file means you only ever edit styles in one place.
- Each article page has structured data (JSON-LD) and unique meta title/description already in the `<head>` — no extra SEO plugin needed.
- The `images/` folder is already referenced correctly — just drop your generated images in and they'll appear.
