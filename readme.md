# PWA Studio good-to-know information

## Get Started / Customize

- [Getting started with Magento PWA Studio](https://larsroettig.dev/getting-started-with-magento-pwa-studio)
- [Getting started with PWA Studio Extensibility](https://larsroettig.dev/getting-started-with-pwa-studio-extensibility)
- [How to extend PWA Studio with new features](https://marcin-kwiatkowski.com/how-to-extend-pwa-studio-with-new-features)
- [Simplifying styling in PWA Studio](https://dev.to/chrisbrabender/simplifying-styling-in-pwa-studio-1ki1)
- [Simplifying Targetables in PWA Studio](https://dev.to/chrisbrabender/simplifying-targetables-in-pwa-studio-p8b)
- [How to add support for Category Landing Pages to PWA Studio](https://marcin-kwiatkowski.com/how-to-add-support-for-category-landing-pages-to-pwa-studio)
- ["How to build a high-quality PWA Studio extension" OR "How to use the PWA Studio extension generator"](https://marcin-kwiatkowski.com/how-to-build-a-high-quality-pwa-studio-extension)
- [Example of extending CMS page title using talon wrapping](https://github.com/Atwix/pwa-studio-examples/pull/1/files)

## CORS/Caching
- https://fooman.com/blog/magento-2-graphql-getting-off-cors.html

## SEO

- [Server-Side vs Client-Side Rendering And Changing SEO Practices](https://magento.com/blog/technical/server-side-vs-client-side-rendering-and-changing-seo-practices)
- [PWA Studio Content rendering approach](https://magento.github.io/pwa-studio/technologies/basic-concepts/content-rendering/)
- 📹 [How to install Rendertron for Magento PWA Studio to use SSR (Server-side Rendering)](https://www.youtube.com/watch?v=Ux0G80zPcuA)
- SSR Tools:
   - [prerender.io](prerender.io)
   - [seosnap.io](seosnap.io)


## Tips&Tricks

##### Linking to a static file

ℹ️ The information has been taken from the #pwa Slack channel.

💡 _Thanks to Kristof Ringleff, Fooman for the question and possible workaround._

> Q: I am trying to link to a static pdf file. It's fine on upward as I can curl the file url directly. However when I add a link to a page to download this file react-router kicks in. As it's not a defined route useMagentoRoute kicks in and queries the back-end urlResolver for it which doesn't know about the file ending up as a 404. Any thoughts on how to tackle this? Ideally without having to teach the backend new tricks.

> A: Used `<Link>` so far and changing it to just `<a>` seems to avoid the issue.
