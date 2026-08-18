# Empower Church Website

A professional website for Empower Church - providing technology solutions to faith communities. This website includes Home, Privacy Policy, and Terms of Service pages, and is hosted on GitHub Pages with a custom domain.

## Files Included

- `index.html` - Home page showcasing services
- `privacy-policy.html` - Privacy policy page
- `terms-of-service.html` - Terms of service page
- `style.css` - Responsive styling for all pages
- `README.md` - This file

## Features

- ✅ Responsive design (mobile, tablet, desktop)
- ✅ Dark mode support
- ✅ Professional and clean UI
- ✅ Fast loading times
- ✅ SEO-friendly structure
- ✅ Accessible navigation

## Setup Instructions

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in to your account
2. Click the **+** icon in the top right and select **New repository**
3. Name your repository: `empowerchurch.in` (or `username.github.io` if you want it as your main site)
4. Add a description: "Technology solutions for faith communities"
5. Choose **Public** (required for GitHub Pages)
6. Click **Create repository**

### Step 2: Upload Website Files

1. In your new repository, click **Add file** → **Upload files**
2. Upload all files:
   - `index.html`
   - `privacy-policy.html`
   - `terms-of-service.html`
   - `style.css`
3. Add a commit message: "Initial website upload"
4. Click **Commit changes**

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Scroll to the **Pages** section (left sidebar)
3. Under "Build and deployment":
   - Source: Select **Deploy from a branch**
   - Branch: Select **main** (or **master**)
   - Folder: Select **/(root)**
4. Click **Save**
5. Wait 1-2 minutes for GitHub Pages to build your site
6. You'll see a message: "Your site is published at: `https://username.github.io/empowerchurch.in`"

### Step 4: Configure Custom Domain (empowerchurch.in)

#### In GoDaddy:

1. Log in to your GoDaddy account
2. Go to **My Products** → **Domains**
3. Find **empowerchurch.in** and click on it
4. Click **DNS** or **Manage DNS**
5. You'll see DNS records. Look for or add these **A records**:

   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   TTL: 3600
   
   Type: A
   Name: @
   Value: 185.199.109.153
   TTL: 3600
   
   Type: A
   Name: @
   Value: 185.199.110.153
   TTL: 3600
   
   Type: A
   Name: @
   Value: 185.199.111.153
   TTL: 3600
   ```

6. Also add a **CNAME record** for www subdomain:
   ```
   Type: CNAME
   Name: www
   Value: username.github.io (replace 'username' with your GitHub username)
   TTL: 3600
   ```

7. Save the DNS changes

#### In GitHub Repository:

1. Go to repository **Settings** → **Pages**
2. Under "Custom domain", enter: `empowerchurch.in`
3. Click **Save**
4. GitHub will automatically verify the domain and enable HTTPS
5. Check **Enforce HTTPS** once it's available

### Step 5: Verify Setup

- DNS changes can take 24-48 hours to propagate
- You can check status at: [dnschecker.org](https://dnschecker.org)
- Once propagated, visit `https://empowerchurch.in` in your browser

## Local Testing (Optional)

To test the website locally before uploading:

1. Save all HTML, CSS files to a folder
2. Double-click `index.html` to open in your browser
3. Or use a local server:
   ```bash
   python -m http.server 8000
   ```
   Then visit `http://localhost:8000` in your browser

## Customization

### Update Contact Information

Edit the contact section in:
- `index.html` - Change email and phone in the "Get Started" section
- `privacy-policy.html` - Update contact info in section 10
- `terms-of-service.html` - Update contact info in section 13

### Update Colors

Edit `style.css` - Change CSS variables in `:root`:
```css
--primary-color: #2563eb;      /* Main blue color */
--primary-dark: #1e40af;       /* Darker blue for hover */
--text-color: #1f2937;         /* Text color */
```

### Update Content

Edit any HTML file to change:
- Service descriptions
- About section text
- Footer information

## Maintenance

### Regular Tasks:
- Keep privacy policy and terms updated
- Monitor contact form submissions
- Check website analytics (via GitHub)
- Update service descriptions as needed

### Backup:
- GitHub automatically backs up your repository
- All changes are tracked in Git history

## Troubleshooting

### Domain not working:
- Wait 24-48 hours for DNS propagation
- Check DNS records are correct in GoDaddy
- Verify GitHub Pages is enabled in repository settings

### Website looks broken:
- Clear browser cache (Ctrl+Shift+Delete)
- Check browser console for errors (F12)
- Verify all files are uploaded to the repository

### HTTPS not enforcing:
- Wait for GitHub SSL certificate (can take a few minutes)
- Ensure custom domain is properly set in GitHub Pages settings

## Support

For questions about:
- **GitHub Pages:** [GitHub Docs](https://docs.github.com/en/pages)
- **GoDaddy DNS:** Contact GoDaddy support
- **Website content:** Edit the HTML files directly

## License

This website template is provided as-is for your use. Customize as needed for your organization.

---

**Created:** August 2026
**Updated:** August 2026