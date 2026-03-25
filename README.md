# Peak 3 Visuals — Single Property Website

## Deploy to Vercel

### Option 1: Drag & drop (fastest)
1. Go to **vercel.com** → sign up / log in
2. Click **"Add New Project"** → **"Import Third-Party Git Repository"** or just drag this entire folder onto the dashboard
3. It deploys automatically — done

### Option 2: Vercel CLI
```bash
npm i -g vercel
cd vercel-template
vercel
```
Follow the prompts. Your site will be live at `your-project.vercel.app`

### Connect a custom domain
1. In Vercel dashboard → your project → **Settings → Domains**
2. Add your domain (e.g. `2003-102nd-pl.peak3homes.com`)
3. Update DNS as Vercel instructs (CNAME record)

## How to reuse for a new listing

1. Open `public/index.html`
2. Replace:
   - **Address** in the hero section
   - **Stats** (price, beds, baths, sqft)
   - **Description** text
   - **Features** grid
   - **Photo URLs** in the gallery + lightbox JS array
   - **Vimeo video ID** in both hero and video sections
   - **Google Maps embed** coordinates
   - **School info** if different area
   - **Agent contact** info
3. Deploy again — new site in 30 seconds

## File structure
```
vercel-template/
├── vercel.json          ← Vercel config
├── README.md            ← This file
└── public/
    ├── index.html       ← The property website
    └── logo.png         ← Peak 3 Visuals logo
```
