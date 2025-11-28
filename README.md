# Construction PMM Website

Static website built with Webflow and deployed on Vercel.

## Repository
- GitHub: https://github.com/Wrivard/pmm
- Branch: main

## Deployment

### Vercel Setup
1. Go to [vercel.com](https://vercel.com) and sign in
2. Click "Add New Project"
3. Import the GitHub repository: `Wrivard/pmm`
4. Configure deployment settings:
   - **Framework Preset**: Other / Static Site
   - **Build Command**: Leave EMPTY
   - **Output Directory**: Leave EMPTY
   - **Root Directory**: Leave EMPTY

### Environment Variables (To Configure Later)
When ready to enable email functionality, add these in Vercel Dashboard → Settings → Environment Variables:
- `RESEND_API_KEY`: Your Resend API key from resend.com
- `FROM_EMAIL`: Your verified domain email (e.g., noreply@yourdomain.com)

## Project Structure
- `/` - Static HTML pages
- `/css` - Stylesheets
- `/js` - JavaScript files
- `/images` - Image assets
- `/videos` - Video assets
- `/api` - Serverless functions (placeholder for email integration)

## Next Steps
1. Deploy to Vercel following the steps above
2. Configure custom domain (optional)
3. Set up Resend account and verify domain
4. Configure email integration (see `(1)Initial-setup.md` for details)

## Technologies
- Webflow (design/export)
- Vercel (hosting)
- Resend API (email - to be configured)

## Files Created for Deployment
- `package.json` - Node.js dependencies
- `vercel.json` - Vercel configuration (clean URLs)
- `.gitignore` - Git ignore rules
- `api/submit-form.js` - Placeholder email API endpoint
