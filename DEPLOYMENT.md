# Quick Deployment Guide 🚀

## Option 1: GitHub Pages (Recommended - Free)

1. **Create GitHub Repository**:
   - Go to [github.com](https://github.com) and sign in
   - Click "New repository"
   - Name it `birthday-disha` (or any name you prefer)
   - Make it public
   - Don't initialize with README (we already have files)

2. **Upload Files**:
   - Click "uploading an existing file"
   - Drag and drop ALL files from this folder:
     - `index.html`
     - `README.md`
     - `favicon.ico`
     - `assets/` folder (with all images and styles.css)
     - `pages/` folder (with memories.html and notes.html)

3. **Enable GitHub Pages**:
   - Go to repository Settings
   - Scroll to "Pages" section
   - Source: "Deploy from a branch"
   - Branch: "main"
   - Folder: "/ (root)"
   - Click Save

4. **Your site will be live at**: `https://yourusername.github.io/birthday-disha`

## Option 2: Netlify (Super Easy - Free)

1. Go to [netlify.com](https://netlify.com)
2. Drag and drop your entire project folder
3. Get instant deployment with a custom URL
4. Optional: Change the site name in site settings

## Option 3: Vercel (Modern & Fast - Free)

1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub
3. Import your repository
4. Deploy with one click

## Option 4: Firebase Hosting (Free)

```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login to Firebase
firebase login

# Initialize hosting
firebase init hosting

# Deploy
firebase deploy
```

## Testing Locally

To test your website before deploying:

1. **Simple HTTP Server** (if you have Python):
   ```bash
   python -m http.server 8000
   ```
   Then visit: `http://localhost:8000`

2. **Live Server** (VS Code extension):
   - Install "Live Server" extension
   - Right-click on `index.html`
   - Select "Open with Live Server"

3. **Node.js Server**:
   ```bash
   npx serve .
   ```

## File Structure Check

Make sure your project has this structure:
```
Birthday/
├── index.html          ← Main page
├── favicon.ico         ← Website icon
├── README.md           ← Documentation
├── assets/
│   ├── styles.css      ← All styling
│   └── IMG-*.jpeg      ← All photos
└── pages/
    ├── memories.html   ← Photo gallery
    └── notes.html      ← Special notes
```

## Troubleshooting

- **Images not loading**: Check that all image files are in the `assets/` folder
- **Styling broken**: Ensure `styles.css` is in the `assets/` folder
- **Links not working**: Verify all file paths are correct
- **Mobile issues**: Test on different screen sizes

## Custom Domain (Optional)

Most hosting services allow custom domains:
- GitHub Pages: Add CNAME file
- Netlify: Domain settings
- Vercel: Domain configuration

---

Your beautiful birthday website is ready to go live! 🎉
