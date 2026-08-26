# 10Best - Product Review Website

A modern static website for product reviews and recommendations.

## Features

- Responsive design (mobile-first)
- Homepage with hero, categories, featured products, and newsletter
- About page
- Contact page with form
- Blog listing and 3 article pages
- Smooth scrolling and mobile menu
- No build step required - pure HTML/CSS/JS

## Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom styles with CSS variables, no external framework needed
- **Vanilla JavaScript** - Mobile menu toggle and form handling
- **Unsplash** - Free product images

## Deploy to Cloudflare Pages

### Option 1: GitHub + Cloudflare Pages (Recommended)

1. Create a new GitHub repository and push this code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/10best-website.git
   git push -u origin main
   ```

2. Go to [Cloudflare Dashboard](https://dash.cloudflare.com/) → **Pages** → **Create a project**
3. Select **GitHub** and choose your repository
4. Build settings:
   - Framework preset: **None**
   - Build command: *(leave empty)*
   - Build output directory: `/`
   - Environment variables: *(none needed)*
5. Click **Save and Deploy**

### Option 2: Direct Upload

1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com/) → **Pages** → **Create a project**
2. Select **Direct Upload**
3. Drag and drop the entire project folder
4. Configure your custom domain if needed

## Local Development

No build tool needed. Just open `index.html` in your browser:

```bash
# Using Python (any version)
python -m http.server 8000
# Then open http://localhost:8000

# Or using Node.js
npx serve .
```

## File Structure

```
10best-website/
├── index.html          # Homepage
├── about.html          # About page
├── contact.html        # Contact page with form
├── blog.html           # Blog listing
├── blog-post-1.html    # Laptop review article
├── blog-post-2.html    # Wireless earbuds review
├── blog-post-3.html    # Smart home devices review
├── css/
│   └── styles.css      # All styles
├── .github/
│   └── workflows/
│       └── deploy.yml  # (optional) GitHub Actions
└── README.md
```

## Customization

- **Colors**: Edit CSS variables in `css/styles.css` (`:root`)
- **Content**: Edit text directly in each HTML file
- **Images**: Replace Unsplash URLs with your own images
- **Contact form**: Connect to a backend service like Formspree, Netlify Forms, or EmailJS

## License

MIT