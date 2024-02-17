_This resource is still in progress!_

# How to deploy your apps for free <!-- omit in toc -->

A resource for the Columbus Code & Coffee presentation.

### Table of Contents

- [What are the different ways to deploy a web app?](#what-are-the-different-ways-to-deploy-a-web-app)
  - [Traditional "always on" applications](#traditional-always-on-applications)
    - [Traditional hosting providers](#traditional-hosting-providers)
  - [What about "serverless" apps?](#what-about-serverless-apps)
  - [Deploying to the edge](#deploying-to-the-edge)
  - [Static sites](#static-sites)
- [What options do I have to host my database?](#what-options-do-i-have-to-host-my-database)
- [Alternatives to Platform as a Service (PaaS)](#alternatives-to-platform-as-a-service-paas)
  - [Self-hosted PaaS options (deploy to a VPS)](#self-hosted-paas-options-deploy-to-a-vps)
  - [VPS options](#vps-options)
- [Other considerations](#other-considerations)
- [Other resources](#other-resources)

## What are the different ways to deploy a web app?

### Traditional "always on" applications

- Most expensive to host
- Most expensive to scale
- Usually deployed in a single region as a single instance (less capable for concurrent loads)
- More flexible
- More control
- Least barrier to entry

#### Traditional hosting providers

| Provider                        | Pricing                                                                               | Requires Credit Card? |
| ------------------------------- | ------------------------------------------------------------------------------------- | --------------------- |
| [Railway](https://railway.app/) | [free](https://railway.app/pricing) ($5/m, $5/m credit)                               | Yes                   |
| [Fly](https://fly.io/)          | [free](https://fly.io/docs/about/pricing/)                                            | Yes                   |
| [Render](https://render.com/)   | [free](https://render.com/pricing) ([limited per user](https://docs.render.com/free)) | No                    |
| [Glitch](https://glitch.com/)   | [free](https://glitch.com/pricing) (apps sleep after 5 minutes)                       | No                    |

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

## What options do I have to host my database?

Apps often need a database to persist non-static data. Many hosts offer a database as a service, but there are also options for hosting your database separately from your app.

- [Supabase](https://supabase.com/)
- [Firebase Firestore](https://firebase.google.com/docs/firestore/quickstart)
- [Cloudflare D1](https://developers.cloudflare.com/d1/)

## Alternatives to Platform as a Service (PaaS)

### Self-hosted PaaS options (deploy to a VPS)

- [Coolify](https://coolify.io/)
- [Dokku](https://dokku.com/)

### VPS options

- [Digital Ocean](https://www.digitalocean.com/)
- ???

## Other considerations

- Authentication & Authorization
  - Auth0
  - Clerk
  - Firebase
  - Supabase
- CI/CD
  - GitHub Actions
  - GitLab CI
  - CircleCI
- Monitoring
  - UptimeRobot
  - Pulsetic
- Logging
  - Datadog
  - Sumologic
- Error tracking
  - Sentry
  - AppSignal
  - BugSnag
- Runtime testing
  - Playwright
  - Cypress

## Other resources

- [Syntax: Own your own PaaS](https://syntax.fm/show/730/own-your-own-paas)
