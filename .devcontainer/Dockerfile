FROM mcr.microsoft.com/vscode/devcontainers/go:1.18

RUN curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s -- -b $(go env GOPATH)/bin v1.46.2

RUN go install github.com/cosmtrek/air@latest

RUN chown -R vscode /$GOPATH
