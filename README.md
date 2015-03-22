Simple go web app
=================

This is a simple demonstration web app written in Go (martini framework) that easily runs on Cloud Foundry.

Locally
-------

```
go run main.go
```

Or to set the message:

```
MESSAGE="this is the message to display" go run main.go
```

Cloud Foundry
-------------

```
cf push myapp --no-start
cf set-env myapp MESSAGE "this is myapp"
cf start myapp
```
