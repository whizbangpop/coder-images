---
name: NodeJS Image
description: Create a basic NodeJS workspace - based on a Docker cotnainer.
tags: [local, docker, nodejs]
icon: /icon/docker.png
---

# NodeJS

To get started, run `coder templates create` and follow the onscreen prompts.

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
