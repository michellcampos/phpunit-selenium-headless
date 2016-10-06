docker-phpunit-selenium-headless
===================================

A Dockerfile starting a selenium standalone server with Chrome and Firefox beta.

It exposes:
- selenium standalone server running on `localhost:4444`
- vnc server running on `localhost:5999`, password: `secret`

Running:

```shell
docker pull michellcampos/phpunit-selenium-headless
docker run --privileged -p 4444:4444 -p 5999:5999 -v (path test suite):/testes -d michellcampos/phpunit-selenium-headless
```
