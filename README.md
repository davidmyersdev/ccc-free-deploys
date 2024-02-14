# How to deploy your apps for free <!-- omit in toc -->

A resource for the Columbus Code & Coffee presentation.

### Table of Contents

- [What are the different ways to deploy a web app?](#what-are-the-different-ways-to-deploy-a-web-app)
  - [Traditional "always on" applications](#traditional-always-on-applications)
  - [What about "serverless" apps?](#what-about-serverless-apps)
  - [Deploying to the edge](#deploying-to-the-edge)
  - [Static sites](#static-sites)

## What are the different ways to deploy a web app?

### Traditional "always on" applications

- Most expensive to host
- Most expensive to scale
- Usually deployed in a single region as a single instance (less capable for concurrent loads)
- More flexible
- More control
- Least barrier to entry
- Examples:
  - [Railway](https://railway.app/)
  - [Fly](https://fly.io/)
  - [Render](https://render.com/)
  - [Glitch](https://glitch.com/)

### What about "serverless" apps?

- Quite a bit less expensive to host
- Can be less expensive to scale
- Decent user experience for users in a closer region, but often not deployed close to users around the world
- Can handle concurrent loads better than traditional hosting
- Less runtimes available
- Slightly higher barrier to entry
- Although the name implies otherwise, there are still servers involved
- Examples:
  - [Firebase](https://firebase.google.com/)
  - [Vercel](https://vercel.com/)
  - [Netlify](https://www.netlify.com/)

### Deploying to the edge

- Way less expensive to host
- Way less expensive to scale
- Better user experience (faster loads times, lower latency, etc) since code is deployed to many locations close to users
- Least amount of runtimes available
- Much higher barrier to entry
- Often runs "raw" JavaScript (no Node)
- Examples:
  - [Cloudflare Workers](https://pages.cloudflare.com/)
  - [Vercel](https://vercel.com/)
  - [Netlify](https://www.netlify.com/)

### Static sites

- The cheapest to host
- The cheapest to scale
- The most limited (only static assets, no server)
- Limited to technologies that run in a web browser
- You can't run a server, and you can't authenticate your users without a third-party service (more on that later).
- Examples:
  - [GitHub Pages](https://pages.github.com/)
  - [Vercel](https://vercel.com/)
  - [Netlify](https://www.netlify.com/)
  - [Cloudflare Pages](https://pages.cloudflare.com/)
