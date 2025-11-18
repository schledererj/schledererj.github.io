# schledererj.github.io

Houses Jack Schlederer's personal website.

## Local development

To run the local server, make sure Docker is installed, comment/uncomment the relevant lines in `_config.yml`, then run the following Docker command:

```powershell
docker run --rm `
  --volume="${PWD}:/srv/jekyll:Z" `
  --volume="${PWD}/local_cache:/usr/local/bundle" `
  --publish 4000:4000 `
  jekyll/jekyll:3 `
  jekyll serve --config _config_local.yml
```