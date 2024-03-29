# .

Welcome, lets get started with your new Tanzu plugin repository.

## Getting Started
First, run `make init` to ensure your plugins go.sum is generated.

## Generate a plugin
Add a plugin with the tanzu cli: `tanzu builder cli add-plugin myplugin`

## Directory Structure

artifacts/: Where you plugins build output will be located

cmd/plugin/<plugin>: Path where you plugins main directory will live

cmd/plugin/<plugin>/test: Plugins are required to have a test command defined

## Commands

`make build`: builds your plugin artifacts
`make lint`: run the golangci linter on your plugin code

## Private Repos
Until the repository is open sourced, you will have to set PRIVATE_REPOS for gomodules to work properly.
```
export PRIVATE_REPOS="github.com/vmware-tanzu/tanzu-framework"
```
