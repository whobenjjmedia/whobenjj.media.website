# whobenjj.com – GitHub Pages site

Files in this folder:
- index.html (home), photography/index.html, design/index.html
- images/ (all compressed photos and designs)
- CNAME (tells GitHub to serve the site at whobenjj.com)
- robots.txt and sitemap.xml (for Google)

## Set up
1. Create a free GitHub account, then a new PUBLIC repository (for example "whobenjj-site").
2. Upload everything in this folder to the repository root (Add file > Upload files). index.html must be at the top level.
3. Repository Settings > Pages > Build and deployment: Source "Deploy from a branch", Branch "main", folder "/ (root)", Save.
4. Same page, "Custom domain": type whobenjj.com and Save (do this BEFORE changing DNS).
5. At your domain provider, add these DNS records (remove any old A or CNAME records for @ and www first):
   A      @    185.199.108.153
   A      @    185.199.109.153
   A      @    185.199.110.153
   A      @    185.199.111.153
   CNAME  www  YOUR-GITHUB-USERNAME.github.io
   (Optional IPv6: AAAA @ 2606:50c0:8000::153, 8001::153, 8002::153, 8003::153)
6. Wait up to 24 hours, then tick "Enforce HTTPS" in Settings > Pages.
7. Optional but recommended: Settings > Pages > "Add a domain" to verify whobenjj.com with a TXT record.
