---
title: "Hosting on Github"
date: 2023-10-08T01:15:57+05:30
draft: true
Author: "Murali Ramu"
toc:
---


This are the steps which I followed to bring up my website.
## mirutech.dev
One can get started by building their website on Hugo. From a Windows user perspective, all that needs to be done is download the binary from [git](https://github.com/gohugoio/hugo/releases/tag/v0.118.0) and add the location to the environment variables of your systems. Then follow Hugo's [quick start guide](https://gohugo.io/getting-started/quick-start/). In the getting started guide hugo.toml is used, but based on the theme, that I was using, I changed it to config.yaml. Once you are done with building the content needed for your webpage using Hugo, you can follow the steps mentioned [here](https://gohugo.io/hosting-and-deployment/hosting-on-github/). This will help you get a webpage up and running with a 'github.io' link.

If you have a custom domain which you'd like to use, then [this doc](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages) will be helpful.


## resume.mirutech.dev
I created a subdomain like the above by adding a CNAME record at the top of the repo. Since this was based on [jsonresume](https://jsonresume.org/), I created a resume.json file, added [github workflows](https://github.com/mirutech2/resume/blob/main/.github/workflows/pages.yml) and add the custom domain under pages of the repo settings.