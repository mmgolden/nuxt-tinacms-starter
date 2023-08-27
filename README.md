# Nuxt Tina CMS Starter

A starter template for Nuxt 3, Nuxt Content, and Tina CMS

## Features

- [Nuxt 3](https://nuxt.com/)
- [Nuxt Content](https://content.nuxtjs.org/)
- [Tina CMS](https://tina.io/)
- [Netlify functions](https://www.netlify.com/products/functions/)
- Media management with [Cloudinary](https://cloudinary.com/)
- TypeScript
- ESLint
- Prettier

## Getting started

### Local development

Create a new file called .env and copy the contents of .env.example to that file.

You will need a Tina Cloud account and a Cloudinary account. Add your keys to the .env file.

Install dependencies

`npm install`

Start the dev server

`npm run dev`

Open the site at http://localhost:3000

To access Tina CMS locally, go to http://localhost:3000/admin/

### Netlify functions

Use the Netlify CLI to run the Netlify function locally and use the media manager. See the [installation documentation](https://docs.netlify.com/cli/get-started/#installation).

Test Netlify functions locally

`netlify dev`

Open the site at http://localhost:8888

To access Tina CMS and the media manager locally, go to http://localhost:8888/admin/

### Deployment

Generate a static site

`npm run generate`
