# GitHub
Everything I have learnt so far in GitHub!

## Deploying projects with GitHub Pages
1. Set base in vite.config.js  

   -  `base: '/<REPO>/'`  
    If deploying to `https://<USERNAME>.github.io/<REPO>` (the repository is located at `https://github.com/<USERNAME>/<REPO>`)  

    - `base: '/'`  
    If deploying to custom domain or `https://<USERNAME>.github.io/`  
      

2. In repository settings, under GitHub Pages, change source of deployment to "GitHub Actions". Follow prompt to create workflow. Sample workflow using npm can be found in link. Remember to change file type to .yml.

  *Source: https://vitejs.dev/guide/static-deploy.html#github-pages*