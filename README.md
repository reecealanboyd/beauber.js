# beauber.js

### Editors and Configuration
Code consistency for this project is maintained via [EditorConfig](https://editorconfig.org). The configuration that EditorConfig uses for this project is located in the root level file [.editorconfig](https://github.com/reecealanboyd/beauber.js/blob/master/.editorconfig).
If using [Visual Studio Code](https://code.visualstudio.com) (recommended), you can find the [EditorConfig plugin for VS Code](https://marketplace.visualstudio.com/itemdetails?itemName=EditorConfig.EditorConfig) by entering `ext install EditorConfig` in VS Code's Quick Open (⌘P).

### Package Management
Package management for this project is handled via [npm](https://www.npmjs.com). Packages being managed for this project are located in the root level file [package.json](https://github.com/reecealanboyd/beauber.js/blob/master/package.json). After cloning the project, you can install the packages shown there by running `npm install` in the root level of the project.

### Development Web Server
You can run the project on your local machine's port 3000 with [Express](https://expressjs.com/) by running the command `npm buildScripts/srcServer.js`. You can then use [localtunnel](https://github.com/localtunnel/localtunnel) to allow others to access the running instance on your machine. If necessary, install localtunnel using the command `npm install -g localtunnel`. Then expose a URL for others to visit by using the command `lt --port 3000`. Optionally, you can provide a subdomain instead of the randomly generated one using by adding `--subdomain <the-domain-you-want>`.

### Automation
[NPM Scripts](https://docs.npmjs.com/misc/scripts) is used for automation within this project via the `scripts` section of [package.json](https://github.com/reecealanboyd/beauber.js/blob/master/package.json). The previous commands to deploy to local tunnel with the prefiix "beauber" have been simplified to `npm run share`. Additionally, local development can be run more simply with `npm start`.

### Transpiling
Transpilation from ES6 to ES5 code supported most by most browsers is possible due to [Babel](https://babeljs.io/). You can see the Babel configuration for this project in [.babelrc](https://github.com/reecealanboyd/beauber.js/blob/master/.babelrc).

### Bundling
This project uses [Webpack](https://webpack.js.org/) for bundling. You can view the configuration for Webpack in this project via [webpack.config.dev.js](https://github.com/reecealanboyd/beauber.js/blob/master/webpack.config.dev.js).
