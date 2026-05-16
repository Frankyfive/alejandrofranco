# Alejandro Franco - CFO Portfolio

A single-page portfolio website for Alejandro Franco, CFO at Cairn Real Estate Holdings.

## Project Structure

```
/
├── index.html          # Main page
├── style.css           # Stylesheet
├── CNAME               # Custom domain (add when ready)
├── images/
│   ├── hero.jpg        # Arms-crossed hero photo
│   ├── headshot.jpg    # Blue tie close-up for About
│   ├── event.jpeg      # NAHREP/L'ATTITUDE event photo
│   ├── award-2025.webp # Finance Leaders 2025
│   └── award-2023.webp # Finance Leaders 2023
└── README.md
```

## Deployment to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name the repo (e.g., `alejandrofranco` or `portfolio`)
3. Set it to **Public**
4. Do NOT initialize with a README (you already have files)

### Step 2: Push the Code

Open your terminal in the project folder and run:

```bash
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repo on GitHub
2. Navigate to **Settings > Pages**
3. Under "Source," select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**
6. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/`

### Step 4: Add a Custom Domain (When Ready)

1. In **Settings > Pages**, enter your custom domain (e.g., `alejandrofranco.com`)
2. Create a file called `CNAME` in the root of your repo with just the domain:
   ```
   alejandrofranco.com
   ```
3. Update your domain's DNS settings:
   - For an apex domain (`alejandrofranco.com`), add these A records:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - For a `www` subdomain, add a CNAME record pointing to `YOUR_USERNAME.github.io`
4. Check "Enforce HTTPS" in GitHub Pages settings once DNS propagates

## Formspree Setup (Resume Form)

1. Go to [formspree.io](https://formspree.io) and create a free account
2. Create a new form and copy your form endpoint (looks like `https://formspree.io/f/xabcdefg`)
3. In `index.html`, find this line:
   ```html
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
4. Replace `YOUR_FORM_ID` with your actual Formspree form ID
5. Formspree will email you each time someone submits the form
6. You can then manually review and send your resume

### Free Tier Limits
- 50 submissions per month
- Email notifications
- No credit card required

## Customization

### Colors
All colors are defined as CSS variables at the top of `style.css`. The palette is:
- **Navy** (primary): `--navy-800: #0f2038`
- **Gold** (accent): `--gold: #b8945f`
- **Slate** (text): `--slate-600: #475569`

### Fonts
The site uses Google Fonts:
- **Cormorant Garamond** for headings (serif, editorial feel)
- **Outfit** for body text (clean, modern sans-serif)

### LinkedIn
Update the LinkedIn URL in the footer of `index.html` to your actual profile link.
