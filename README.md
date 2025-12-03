# steps to deploy react project to github pages

1. initialize git to your project and add it to the github repository

2. install gh-pages package - 'npm install --save-dev gh-pages' 
(This package enable the root to make the project host)

3. then inside the package.json file add - 
"homepage" : "https://[github username].github.io/[repo name]/"
eg - "homepage": "https://kavitabhoite.github.io/react-sample/"

4. add predeploy and deploy scripts inside the "scripts" section in package.json - 
"deploy": "gh-pages -d dist",
"predeploy": "npm run build"

5. push to the main

6. Now deploy the app - 'npm run deploy'
