Project #5 - viewer+server+oss+derivatives

The setup is similar for those 3 projects and they have to be run independently.

Those projects are using Webpack, a module bundler and NPM packages to build and generate the frontend code, so an extra build step is required.

Navigate with a command shell or terminal to the project you want to run and type the following commands:

Mac OSX/Linux (Terminal)

> npm install
> export NODE_ENV=development
> export FORGE_DEV_CLIENT_ID=<YOUR CLIENT ID FROM DEVELOPER PORTAL>
> export FORGE_DEV_CLIENT_SECRET=<YOUR CLIENT SECRET>
> npm start (builds the client dynamically in memory using webpack dev server)
Windows (use Node.js command line from Start menu)

> npm install
> set NODE_ENV=development
> set FORGE_DEV_CLIENT_ID=<YOUR CLIENT ID FROM DEVELOPER PORTAL>
> set FORGE_DEV_CLIENT_SECRET=<YOUR CLIENT SECRET>
> npm start (builds the client dynamically in memory using webpack dev server)
Open your browser at: http://localhost:3000

To run a production build you can use build command:

> npm run build
A production build code is minified and function names are mangled which make it much smaller and impractical for debugging or reverse engineering.