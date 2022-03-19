# Netlify + NetlifyCMS + TailwindCSS starter for Gridsome

### 1. Install Gridsome CLI tool if you don't have

`npm install --global @gridsome/cli`

### 2. Create a Gridsome project

1. `gridsome create my-gridsome-site https//github.com/esparkman/gridsome-starter-netlify-netlifycms-tailwindcss.git` to generate with this starter
2. `cd my-gridsome-site` to open the folder
3. `gridsome develop` to start a local dev server at `http://localhost:8080`
4. Happy coding 🎉🙌

### Or take the easy route use the Easy Button

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/guifelix/gridsome-starter-netlify-netlifycms-tailwindcss)

### 3. Setting up Github Authentication for NetlifyCMS

Netlify already has some excellent documentation on configuring your newly deployed Application for Github. I'll point you to their Docs for this step of the process. You may have to bounce back and forth between Github and Netlify for this process.

[Gridsome NetlifyCMS Github Authentication](https://gridsome.org/docs/guide-netlify-cms#netlify-cms-authentication-with-github)

### 4. Configuring NetlifyCMS

Once you have completed setting up your Github Authentication it's time to configure NetlifyCMS. It's really only one change. You'll need to modify your repo information. Do this by browsing to `./src/admin/config.yml`.

In this file you will see the following:

```yaml
backend:
  name: github
  repo: esparkman/gridsome-example
```
You will want to update the `repo` node with your github repo information. This will either be the repo you used when using the One Button Deploy or whatever name you used when you generated your Application.

### 5. Start Creating

At this point you should have a fully functional Gridsome Starter up and running. To start using NetlifyCMS to manage your Content, simply browse to <your-hostname>/admin.

Thanks for using this Starter Kit. I'm always happy to receive constructive comments!