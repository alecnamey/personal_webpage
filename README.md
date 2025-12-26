# alecnamey.com

Personal website for Alec Namey - Software Engineer and Computer Science student at UC Santa Cruz.

## 🚀 Deployment to GitHub Pages

This site is deployed to GitHub Pages with a custom domain (`alecnamey.com`).

### Initial Setup

1. **Push your code to GitHub:**
   ```bash
   git add .
   git commit -m "Initial commit for personal website"
   git push origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under **Source**, select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

3. **Set up custom domain:**
   - The `CNAME` file is already included in this repo
   - GitHub will automatically detect it and configure the domain
   - You'll need to configure DNS records with your domain registrar:
     - **Type:** `CNAME`
     - **Name:** `@` (or `www` if you want www.alecnamey.com)
     - **Value:** `alecnamey.github.io` (or `yourusername.github.io` if different)
   - For the root domain (`alecnamey.com`), you may need to use:
     - **Type:** `A` records pointing to GitHub's IPs:
       - `185.199.108.153`
       - `185.199.109.153`
       - `185.199.110.153`
       - `185.199.111.153`

4. **Wait for DNS propagation** (can take up to 24-48 hours)

5. **Enable HTTPS:**
   - GitHub Pages will automatically provision an SSL certificate once DNS is configured
   - This may take a few minutes to a few hours

### Local Development

To test the site locally:

```bash
python3 -m http.server 5500
```

Then open `http://localhost:5500` in your browser.

## 📁 Project Structure

- `index.html` - Main HTML file
- `styles.css` - All styling
- `IMG_9297.jpeg` - Profile picture
- `Alec_s_Resume (5).pdf` - Resume PDF
- `CNAME` - Custom domain configuration for GitHub Pages

## 🛠️ Tech Stack

- Pure HTML/CSS (no frameworks)
- Responsive design
- Modern CSS with glassmorphism effects
