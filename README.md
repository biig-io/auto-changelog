Automatically generates CHANGELOG of your git repository.

It is a container to execute auto-changelog npm package on Alpine independently of your technical stack.

Versions match auto-changelog npm package version.

Check [auto-changelog repository](https://www.npmjs.com/package/auto-changelog) for more information about available options.

# Examples

## Launch latest

`docker run -it --rm -v "$(pwd)":/usr/local/src/your-app biig/auto-changelog -t keepachangelog -u -o CHANGELOG.md --tag-pattern .+ --include-branch master --release-summary`

## Launch specific version (e.g. 1.11.0)

`docker run -it --rm -v "$(pwd)":/usr/local/src/your-app biig/auto-changelog:1.11.0 -t keepachangelog -u -o CHANGELOG2.md --tag-pattern .+ --include-branch master --release-summary`
