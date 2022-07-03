# artifactory
The repo to host self-update binaries for golang projects

Some useful commands:

```bash
go build -ldflags="-X main.version=1.1" -o hello-updater src/hello-updater/main.go
```

```bash
go-selfupdate -o public/hello-updater/ hello-updater 1.1
```

```bash
go build -ldflags="-X main.version=1.2" -o hello-updater src/hello-updater/main.go
```

```bash
go-selfupdate -o public/hello-updater/ hello-updater 1.2
```
