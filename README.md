# Nodedock

Docker NodeJS development environment.

## Goal

I'm an ex-PHP developer, and I've used to use Laradock and similar solutions a lot. However, there's no close thing in NodeJS ecosystem (or at least I didn't find it). So, I decided to build a solution based on Laradock, but for NodeJS. This is how Nodedock was born.

## Usage Example

You need to have a node project with `package.json` with `start` script definition as `node` container will run `npm start` command after start up.

```
cd $NODE_PROJECT_ROOT
git submodule add https://github.com/nodedock/nodedock.git
cp nodedock/env-example nodedock/.env
cd nodedock/
docker-compose up -d nginx node workspace
docker-compose logs -f
```

The last one is optional.

## Based on Laradock

This project is based on awesome [Laradock](https://github.com/laradock/laradock) ([contributors](https://github.com/laradock/laradock/graphs/contributors))

# LICENSE

MIT
