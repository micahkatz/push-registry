# push-registry

A shorthand for pushing a Docker image to a container registry, cleaning up your local images, and creating a github release

## Usage

`push-registry <image-name> [-g -d]`

-   `-g` will create a github release with your specified version. Requires `gh` cli
-   `-d` will delete the associated docker images after pushing to the registry
-   `REGISTRY` environment variable
    -   Pass this in with `REGISTRY=<your/registry/name> push-registry <extra args>`
    -   Pro Tip: set this in your `~/.zshrc` or `~/.bashrc` for easy running
        -   You can also overwrite your default by setting `REGISTRY` manually before you run `push-registry`
