# Auracelle Polaris · GitHub Pages Deployment Guide

## Files Included

Three files are required for GitHub Pages deployment:

1. **index.html** – The complete Polaris wargaming simulation (playable HTML file)
2. **README.md** – Documentation, overview, and links
3. **.nojekyll** – Empty file that tells GitHub Pages to serve files as-is (no Jekyll processing)

## Deployment Instructions

### Option A: Create a New Standalone Repository (Recommended for a dedicated Polaris repo)

1. **Create a new GitHub repository**:
   - Go to [github.com/new](https://github.com/new)
   - Repository name: `Auracelle-Polaris-Space-Domain` (or your preferred name)
   - Description: "Auracelle Polaris · Space Governance Wargaming Intelligence Platform"
   - Make it **Public**
   - Do NOT initialize with README, .gitignore, or license (you already have these)
   - Click "Create repository"

2. **Push the three files to the repository**:
   ```bash
   cd /path/to/Auracelle-Polaris-Space-Domain
   
   # Initialize git if not already done
   git init
   
   # Add all files
   git add index.html README.md .nojekyll
   
   # Commit
   git commit -m "Initial commit: Auracelle Polaris v2.0 wargaming simulation"
   
   # Add remote (replace YOUR-USERNAME and REPO-NAME as needed)
   git remote add origin https://github.com/YOUR-USERNAME/Auracelle-Polaris-Space-Domain.git
   
   # Push to main branch
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click **Settings** (top menu)
   - Scroll down to **Pages** (left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Under "Branch", select **main** and **/root** folder
   - Click **Save**
   - GitHub will show you the live URL in a few moments (typically `https://YOUR-USERNAME.github.io/Auracelle-Polaris-Space-Domain/`)

### Option B: Add Polaris to an Existing Auracelle Suite Repository

If you want to integrate Polaris alongside Charlie, Orion, Lyra, Delphi, etc. in your main Auracelle Suite repo:

1. **Inside your existing Auracelle Suite repository**, create a `polaris/` folder:
   ```bash
   mkdir -p polaris
   cp index.html polaris/index.html
   cp README.md polaris/README.md
   ```

2. **Do NOT place `.nojekyll` inside the `polaris/` folder** — `.nojekyll` should remain at the repository root (alongside your main README, other suite modules, etc.)

3. **Update your main suite README** to add a link:
   ```markdown
   - **[Polaris](polaris/)** – Space governance wargaming
   ```

4. **Push and deploy** as you normally would for the suite repo. Polaris will be accessible at `https://YOUR-USERNAME.github.io/Auracelle-Suite-AI-Governance-Labs/polaris/`

## Live URL After Deployment

Once GitHub Pages is enabled and deployed, Polaris will be live at:

**Standalone repo**: `https://YOUR-USERNAME.github.io/Auracelle-Polaris-Space-Domain/`

**Integrated into suite**: `https://YOUR-USERNAME.github.io/Auracelle-Suite-AI-Governance-Labs/polaris/`

## Verifying Deployment

After pushing, GitHub will:
1. Build the site automatically (takes ~30 seconds – 1 minute)
2. Show a green checkmark in the Actions tab once successful
3. Display the live URL in the Pages settings

If you see a red X in Actions, click on it to view the error. Common issues:
- Missing `.nojekyll` file (though usually not critical for HTML files)
- File path issues (check that `index.html` and `README.md` are at the root)

## Updating Polaris

If you make changes to the simulation:

1. Replace `index.html` with the new version
2. Commit and push:
   ```bash
   git add index.html
   git commit -m "Update Polaris: [describe changes]"
   git push
   ```
3. GitHub Pages will rebuild automatically within 1 minute

## Email to Mr. Hamid Mehmood

Once deployed, you can share the live link with Mr. Mehmood:

> Dear Mr. Mehmood,
>
> Thank you for the opportunity to present at WSIS Forum 2026. I am pleased to share **Auracelle Polaris**, a playable space governance wargaming platform I have developed.
>
> **Live Simulation**: [INSERT YOUR GITHUB PAGES URL HERE]
>
> Polaris models decision-making when space systems are under strategic pressure across five crisis scenarios (Kessler Cascade, GPS Degradation, ASAT Testing, Megaconstellation Governance, Allied Coordination Breakdown). Players make governance and operational moves while Agentic AI actor-agents stress-test each choice, exposing governance-resilience gaps in real time.
>
> For more on my research and the full Auracelle simulation suite:
> - Auracelle Platform: https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public
> - Auracelle Suite: https://auracelle.github.io/Auracelle-Suite-AI-Governance-Labs/
>
> I would welcome the opportunity to discuss how Polaris could support WSIS or future UN space governance initiatives.
>
> Warm regards,
> Grace-Alice Evans

---

## Support & Further Customization

- **Add a custom domain**: In GitHub Pages settings, you can add a custom domain (e.g., `polaris.auracelle.io`)
- **Custom favicon**: Add a `favicon.ico` file to the root directory
- **Disable indexing**: Add `_config.yml` with `plugins: []` if you want to ensure no Jekyll processing

For more on GitHub Pages: https://docs.github.com/en/pages

---

**Questions?** Refer to the GitHub Pages documentation or reach out to GitHub Support.
