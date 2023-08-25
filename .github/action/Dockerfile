FROM node:18-alpine
LABEL "repository"="https://github.com/pkj1993/github-tag-action"
LABEL "maintainer"="prasanna"

RUN apk --no-cache add bash git curl jq && npm install -g semver

COPY entrypoint.sh /entrypoint.sh

RUN chmod +x entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
