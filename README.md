# Hello Dev Container with Python

> Development containers (**Dev Containers**) are a VS Code feature that allows developers to package a local development tool stack into the internals of a Docker container while also bringing the VS Code UI experience with them.

![image](https://github.com/shinyay/hello-devcontainer-with-python/assets/3072734/b0eab7bd-6d6f-49de-a989-3e968dd8d6bb)


## Description

The project consists of the following

```shell
.devcontainer/
├── compose.yaml
└── devcontainer.json
```

```json
{
	"name": "devcontainr_python3",
	"dockerComposeFile": "./compose.yaml",
	"service": "python3",
	"workspaceFolder": "/workspace",
	"shutdownAction": "stopCompose",
	"customizations": {
		"vscode": {
		  "extensions": ["ms-python.python"]
		}
	}
}
```

|item|description|
|----|-----------|
|`name`|Container name visible on VS Code|
|`dockerComposeFile`|Specify by relative path the docker-comopse file used to create the container|
|`service`|Specify the service name of the container you want to open in VScode among the services in docker-compose.yml|
|`workspaceFolder`|Specify the root folder when the container is opened|
|`shutdownAction`|Setting what to do with containers when a container screen is closed in VScode<br>`stopCompose` stops the container when the screen is closed|
|`customizations/vscode/extensions`|Specify VScode extensions to be installed with container creation|

## Demo

## Features

- feature:1
- feature:2

## Requirement

## Usage

## Installation

## References

- [Dev Containers: Getting Started](https://microsoft.github.io/code-with-engineering-playbook/developer-experience/devcontainers/)

## Licence

Released under the [MIT license](https://gist.githubusercontent.com/shinyay/56e54ee4c0e22db8211e05e70a63247e/raw/34c6fdd50d54aa8e23560c296424aeb61599aa71/LICENSE)

## Author

- github: <https://github.com/shinyay>
- twitter: <https://twitter.com/yanashin18618>
- mastodon: <https://mastodon.social/@yanashin>
