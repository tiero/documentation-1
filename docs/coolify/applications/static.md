# Static 
Base docker image: [webdevops/nginx:alpine](https://hub.docker.com/r/webdevops/nginx)

Your application will be served as a static site. 

You can define install or build commands, so it will build it before serving your static site. Think of the following frameworks: React, Astro, Nuxt, SvelteKit, Gatsby, etc.

You can customize the base image with environment variables, see the [docs](https://dockerfile.readthedocs.io/en/latest/content/DockerImages/dockerfiles/nginx.html).