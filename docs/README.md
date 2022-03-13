# Docsify Simple Documentation Template
> Disclaimer: Under development and not ready for automatic usage.

This repo intent to serve a template to create an awesome looking documentation page of markdown files using [docsify.js](https://docsify.js.org/) with few simple steps.

## Features
- Dark Mode Theme switch
- Local development with docker-compose
- Automatic sidebar creation
- Copy button for code boxes
- Pagination Plugin
- Search bar Plugin

## Basic first usage
1. Move all markdown documentation files into a folder `./docs`
1. Copy the `index.html` into `./docs`
1. Add an empty `.nojekyll`-File into `./docs`
1. Create a manual `_sidebar.md` into `./docs` with your wished structure

> To use docker-compose for local development also add `Dockerfile` and  `docker-compose.yml` to your `./docs` directory.

### Local Development
#### Using npm
1. Install docsify-cli: `npm i docsify-cli -g`
1. Run local dev server with: `docsify serve ./docs`

#### Using docker-compose
1. Start docker-compose in detached mode: `docker-compose up -d`
2. View your page at `http://localhost:3000`
3. Stop docker-compose: `docker-compose stop`

> Page reload is necessary to view the updates.

## Deep Dive
### Structure your docs
- It's a good practice to organize your docs into folder for the specific topic.

### Change Name of the Page
Change the name in `index.html` at `window.$docsify = {`

### Use other Plugins or features of docsify
Take a look at the documentation of awesome docsify resources: https://docsify.js.org/#/awesome

### Automatic Sidebar Creation
- Install [hfour/docsify-tools](https://github.com/hfour/docsify-tools) to automatically create a sidebar with CLI
- Add numbers in front of your filenames and folder e.g. `10-readme.md` to let `docsify-tools` create the sidebar in your wished order

### Deploy to GitHub Pages or GitLab Pages
Take a look at the documentation of docsify: https://docsify.js.org/#/deploy.
