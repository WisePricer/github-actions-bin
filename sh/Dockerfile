 FROM node:10-alpine

LABEL "name"="sh"
LABEL "maintainer"="GitHub Actions <support+actions@github.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.name"="Shell for GitHub Actions"
LABEL "com.github.actions.description"="Runs one or more commands in an Action"
LABEL "com.github.actions.icon"="terminal"
LABEL "com.github.actions.color"="gray-dark"

COPY LICENSE README.md THIRD_PARTY_NOTICE.md /

RUN apk --no-cache add zip openssl

COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
