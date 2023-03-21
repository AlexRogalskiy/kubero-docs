---
id: goals-and-concepts
---


# Goals and Concept
Kubero brings the convenience of Heroku/platform.sh/Vercel.dev to your Kubernetes cluster. Your developers should not need to worry about the underlying infrastructure and deployment. Kubero is a tool that helps you to deploy your application in a Kubernetes cluster.

Kubero is basically a Kubernetes Operator with a UI, API, and CLI. It allows you to deploy your application in a Kubernetes cluster without writing any Kubernetes manifests or Dockerfiles.

<img src="https://raw.githubusercontent.com/kubero-dev/kubero/main/docs/img/highlevel.png" />

## CI/CD
You can use it to deploy your application in a Kubernetes cluster. Kubero comes with an integrated CI/CD pipeline, which allows you to deploy your App with a simple push into a branch, or even start a new instance based on a Pull-Request.

The Pipeline does not build a container image. It only pulls your code and runs the build scripts, which are mounted into your running container. Since the Images are not built, pushed, and pulled from a registry, Kubero is a very fast solution.

Nevertheless, you can also deploy already built container images.

## Integrations/Buildpacks

You can run everything that runs in a container. Kubero uses default images to build and run your app. But you can build your own builder if required. And create your custom deployment packs.

- GoLang (including Hugo, gin-gonic)
- Python (including Flask)
- JavaScript/NodeJS
- PHP (including Laravel)
- Ruby (including Rails)
- Static HTML
- Rust (including Rocket)
- ...


You find the preconfigured buildpacks and examples here:
https://github.com/kubero-dev/buildpacks

## Addons/Plugins
Addons are deployed with Kubernetes Operators which are configurable over the UI.

These are the currently available add-ons:
 - Redis
 - Redis cluster
 - MongoDB
 - Postgres

## Articles and Tutorials
 - [Comparing selfhosted Heroku alternatives](https://dev.to/shoksuno/comparing-selfhosted-heroku-alternatives-249p)
 - [The simplest way to run your own Heroku on Kubernetes](https://dev.to/shoksuno/the-simplest-way-to-run-your-own-heroku-on-kubernetes-3l03)
 - [Replace Heroku with Kubero on Kubernetes (part 1)](https://dev.to/shoksuno/replace-heroku-with-kubero-on-kubernetes-2aoj)
