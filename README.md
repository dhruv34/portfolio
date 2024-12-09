Steps to make changes to the website:

1. Add/Edit code
2. In the dhruvsite folder, run: `hugo -t hugo-theme-diary` to generate static assets in the public folder
3. Run `hugo server` to check if the website looks as it should
4. Cd into the public folder which acts as our production repo where we deploy from: `cd public`
5. Git add, commit, and push to dhruv0 branch

Once the static assets are pushed, the changes will auto-deploy in 1-2 minutes!

Other important files:
* hugo.toml - Defines structure of main site
* layouts/index.html - Card layout of main page
* layouts/_default/section.html - Card layout of other pages
* en.yaml - Provides some default text from the Hugo template