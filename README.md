# FinDrive Blog — blog.findrive.ng
## Static HTML — No CMS, No API, No Dependencies

### Deploy to Vercel
1. Go to vercel.com → Add New Project
2. Drag this entire folder into the upload area
3. Click Deploy — live in 60 seconds
4. Add domain: blog.findrive.ng → CNAME blog → cname.vercel-dns.com

---

## How to Add a New Blog Post (5 minutes)

### Step 1 — Open build_blog.py
Find the POSTS list at the top of the file.

### Step 2 — Add your post to the list
Copy this template and fill it in:

```python
{
  'slug': 'your-post-url-slug',          # URL: blog.findrive.ng/your-post-url-slug
  'title': 'Your Post Title Here',
  'excerpt': 'One or two sentence summary shown in the grid card.',
  'category': 'Car Finance',             # One of the 6 categories
  'author': 'FinDrive Team',
  'date': '1 June 2026',
  'read': '5 min read',
  'tags': ['Tag1', 'Tag2', 'Tag3'],
  'featured': False,                     # Set True to show in Featured slot
  'body': """
<p>Your post content here. Use HTML tags.</p>
<h2>A Section Heading</h2>
<p>More content...</p>
<div class="callout"><strong>Tip:</strong> Use callout boxes for key insights.</div>
<ul><li>Bullet point one</li><li>Bullet point two</li></ul>
"""
},
```

### Step 3 — Run the build
```
python3 build_blog.py
```

### Step 4 — Deploy
Drag the folder to Vercel (or push to GitHub if connected).
Your post is live in under 60 seconds.

---

## Categories
- Car Finance
- Insurance  
- Fleet
- Market Updates
- Car Buying Tips
- Company News

## Tracking
- GA4: G-ZX2WN0W064 (all pages)
- Meta Pixel: 1261139099130940 (all pages)
- Share events tracked automatically
- Newsletter signup tracked
