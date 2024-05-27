---
name: 'ArcGIS Online 2: Development environment setup'
about: Get the new team member set up with a complete development environment.
title: Development environment setup
labels: ''
assignees: ''

---

## General Development Environment Setup

- [ ] Install homebrew if you're on a Mac.
- [ ] Install git
  - create a git user
  - add a global `.gitignore` for ignoring things like `DS_Store` files
- [ ] Install editor/terminal of choice (and theme!)
  - Many on the team use VSCode.
- [ ] Install Node/NPM.
  - You can install NVM if you want to easily switch between Node versions.
- [ ] Create an npm account (optional, if needed)
  - Sign in on cli with account
  - Set up two-factor auth for account
  - Email account my way to get added to esri org on npm
- [ ] [Add ssh keys](https://help.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account) to GitHub _and_ Devtopia
- [ ] Create a trusted set of SSL certs (Optional, will allow https local development)
  - [Generating a trusted root certificate](https://gist.github.com/paulcpederson/6e2ff7e85d396e4df007e8a5a00e8a1b) will allow multiple trusted certs to be created

## ArcGIS Online Dev Setup
- [ ] Follow along with the [dev environment setup guide](https://confluencewikidev.esri.com/display/AGO/Dev+Environment+Setup) on confluence. You can also reference the [node server section](https://devtopia.esri.com/WebGIS/arcgis-portal-app#using-the-nodejs-proxy-server) of the README.

After you've gotten everything cloned, all the dependencies installed, the submodules initialized and updated, your hosts file edited, keys generated, and the config setup, you can run a local development server in one of several ways.

- [ ] Run `npm run cfg:dev` to configure your application to connect to the development server (backend).\
- [ ] Run `npm run dev:serve-env` to run the development server.
- [ ] Verify that the server starts up and runs on the correct ports.
- [ ] Verify that your hosts file is correctly configured by visiting `https://local.arcgis.com/home/` (you may see a security warning, just proceed)
  - You can find your hosts file at the following locations given your operating system:
    - Mac: `/private/etc/hosts`
    - Windows: `C:\Windows\System32\drivers\etc\hosts`
    - Linux: `/etc/hosts`
- [ ] Test you can login with these test credentials (username / password): `testCase` / `testtest1`
  - These are temporary credentials. More permanent user accounts will be created for you.

If you run into trouble along the way, just ask! It's a large codebase, so there is a lot to get up to speed on. There are multiple frameworks at play so it can be a little bit confusing to get up to speed initially.
