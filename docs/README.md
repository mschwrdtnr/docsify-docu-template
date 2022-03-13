# Docsify Simple Documentation Template

## Basic first start
1. Move all markdown documentation files into a folder `./docs`
1. Copy the `index.html` into `./docs`
1. Add an empty `.nojekyll`-File into `./docs`
1. Create a manual `_sidebar.md` into `./docs` with your wished structure

### Local Development
#### Using npm
1. Install docsify-cli: `npm i docsify-cli -g`
1. Run local dev server with: `docsify serve ./docs`

#### Using docker-compose
1. Start docker-compose in detached mode: `docker-compose up -d`
1. Stop docker compose: `docker-compose stop`

> Reload the page to view your updates.

## Customizations
### Name of the Page
Change the name in `index.html` at `window.$docsify = {`

### Use other Plugins or features of docsify
Take a look at the documentation of awesome docsify resources: https://docsify.js.org/#/awesome

## Deeper Dive
### Automatic Sidebar Creation
- Install [hfour/docsify-tools](https://github.com/hfour/docsify-tools) to automatically create a sidebar with CLI
- Add numbers in front of your filenames and folder e.g. `10-readme.md` to let `docsify-tools` create the sidebar in your wished order

### Deploy to GitHub Pages or GitLab Pages
Take a look at the documentation of docsify: https://docsify.js.org/#/deploy.
