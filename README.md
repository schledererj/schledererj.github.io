# schledererj.github.io

This repo houses a website where Jack Schlederer posts his musings on various items, including, but not limited to, software engineering, infosec, movies, soccer, data science, and booze (sometimes several at once). There's not much else to see here in the README file other than nerd stuff so get off here and go to the [website!!](https://schledererj.github.io)

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