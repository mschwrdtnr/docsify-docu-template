  FROM mhart/alpine-node:latest
  LABEL description="Dockerfile to serve docsify preview"
  WORKDIR /docs
  COPY . /docs
  RUN npm install -g docsify-cli@latest
  EXPOSE 3000/tcp
  ENTRYPOINT docsify serve .