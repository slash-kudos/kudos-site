# Slash Kudos Website

The Kudos marketing website.

These docs have technical information about how things were setup, where to find stuff, etc. If you're looking for the source for the web app app.slashkudos.com, that would be in [slash-kudos/kudos-web].

Check out the [docs folder](/docs) for more info.

## Quick Reference Guide

- Domain: slashkudos.com
- Hosting: [SiteGround]
- Domain Name Registrar: [Namecheap]
- Framework: Wordpress
- Routing: AWS Route 53

## Site Tools

The marketing site is a Wordpress site. While this may be frowned upon because it's not custom, Wordpress is the easiest way to get a fully customizable yet out-of-the-box solution with templates for landing pages, SEO, content management, blogs, newsletters, and more and I don't want to rebuild that 😄

## Site Hosting

I use SiteGround because I already have an account and it is pretty cheap. You can also grow with it and make it scale reliably.

## Web Site vs Web App

- Site includes the landing page with features explained, prices (not applicable here), contact info, blogs, newsletter sign-ups, etc.
- App is the actual app and can be behind a login or a paywall. In this case this is where you would be able to see the kudos feed and search and give kudos. That code can be found in [slash-kudos/kudos-web]

<!-- Links -->
[slash-kudos/kudos-web]: https://github.com/slash-kudos/kudos-web
[SiteGround]: https://my.siteground.com/websites/list/S3duelpYZ0pJUT09
[Namecheap]: https://www.namecheap.com/
