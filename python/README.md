---
name: Python3
description: Run a basic Python3 (w/Pip3) workspace - based off a Docker container.
tags: [local, docker, python]
icon: /icon/docker.png
---

# docker


To get started, run `coder login <your-coder-url>` to authenticate. 

Then, run `coder templates create`. Follow the on screen prompts.

## Editing the image

Edit the `Dockerfile` and run `coder templates push` to update workspaces.

## code-server

`code-server` is installed via the `startup_script` argument in the `coder_agent`
resource block. The `coder_app` resource is defined to access `code-server` through
the dashboard UI over `localhost:13337`.

## Extending this template

See the [kreuzwerker/docker](https://registry.terraform.io/providers/kreuzwerker/docker) Terraform provider documentation to
add the following features to your Coder template:

- SSH/TCP docker host
- Registry authentication
- Build args
- Volume mounts
- Custom container spec
- More

We also welcome contributions!
