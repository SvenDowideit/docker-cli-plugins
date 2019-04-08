# docker-helloworld

Docker cli hello world cli plugin examples. This repo can be checked out into `~/.docker/cli-plugins`

This repo contains several Docker CLI plugins:
* main.go - `docker-helloworld`: to be built `go build -o docker-helloworld main.go`
* `docker-env` - utterly simplistic bash example that can be run using `docker env`
* `docker-all` - run whatever docker command follows `all` on all swarm nodes (should work in standalone too)
* `docker-prune` - run `docker system prune -f --volumes` on all swarm nodes (should work in standalone too)

main.go comes from https://github.com/docker/cli - in cli-plugins/examples

and then there's a bunch of poking to get a go.mod that lets it build.

now I'm reading https://github.com/docker/cli/issues/1534 - as having the `docker-helloworld` binary in ~/.docker/cli-plugins/ isn't enough
