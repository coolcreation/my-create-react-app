#### Deploy create-react-app project to github - hosted live!
M
Go to github, make new repo named "my-create-react-app"
On pc, create a new folder called "my-create-react-app" and then....
cd my-create-react-app
npm create vite@latest    ( project name is nothing, so type ".")
npm install
npm install -D gh-pages

```js
//edit package.json:
  "homepage": "https://coolcreation.github.io.my-create-react-app/",  // add this line
  "name": "react-vite-website",
  "type": "module",
  "scripts": {
    "predeploy": "npm run build",      // add this line
    "deploy": "gh-pages -d build",        // add this line
    "dev": "vite",
    "build": "vite build",
  },
```
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/coolcreation/my-create-react-app.git
git push -u origin main
npm run deploy


