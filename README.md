# jekyll2nuxt

A jekyll to nuxtjs template with batteries included!!

 * Progressive Web Application.
 * Markdown and front matter supported (it auto-converts it to JSON).
 * Routes generation for your blogposts out of the box.
 * Fully static site, with the perfect SEO.

You can try the demo of this repository here: [https://jekyll2nuxtjs.daniellombrana.es/](https://jekyll2nuxtjs.daniellombrana.es/)

You can check my [personal site](https://daniellombrana.es), that uses this template.

## Build Setup

``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn run dev

# build for production and launch server
$ yarn run build
$ yarn start

# generate static project
$ yarn run generate
```

For detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).

## Importing your Jekyll blogposts

You can import your Jekyll blog posts by just copying them into the content/blogposts folder.

Then re-run yarn run dev or yarn run build to launch it. 

## Deploying to Zeit, Github or any other static site

Basically be sure to know how to deploy the dist folder after running:
 
```
# build static site
$ yarn build
```

You can quickly test it in your machine with python:

```
# run a simple server to test your static site
$ python -m SimpleHTTPServer 8001
```
