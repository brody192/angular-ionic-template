---
title: Angular + Ionic + Caddy
description: The default Ionic Angular starter, utilizing `Caddy` to serve the built single page app
tags:
  - Node
  - Angular 17
  - Ionic
  - Caddy
---

# Ionic + Angular + Caddy

This project was originally generated with [`ionic start`](https://ionicframework.com/docs/developing/starting)

<!-- [![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/13NBfA?referralCode=ySCnWl) -->

## ✨ Features

- Ionic + Angular + Caddy
- Caddy v2

## 💁‍♀️ Local Development

- Install required dependencies with `npm install`
- Run `npm start` for a development server
- Navigate to `http://127.0.0.1:4200/`. The application will automatically reload if you change any of the source files.

To get more help on the Ionic CLI use `ionic help` or go check out the [Introduction to Ionic](https://ionicframework.com/docs/) page.

## ❓ Why use `Caddy` when deploying to Railway?

Caddy is a powerful, enterprise-ready, open source web server, and therefore Caddy is far better suited to serve websites than `ng serve` is, using Caddy will result in much less memory and cpu usage compared to serving with `ng serve` (much lower running costs too)

To see how this is achieved with nixpacks, check out the fully documented nixpacks.toml file in this repository

The configuration for Caddy is called a Caddyfile, and you can edit that file to further suite your needs, by default it comes configured to serve a single page app for Angular, and to also gzip the responses

**Relevant Caddy documentation:**

- [The Caddyfile](https://caddyserver.com/docs/caddyfile)
- [Caddyfile Directives](https://caddyserver.com/docs/caddyfile/directives)
- [root](https://caddyserver.com/docs/caddyfile/directives/root)
- [encode](https://caddyserver.com/docs/caddyfile/directives/encode)
- [file_server](https://caddyserver.com/docs/caddyfile/directives/file_server)
- [try_files](https://caddyserver.com/docs/caddyfile/directives/try_files)