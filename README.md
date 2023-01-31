# Antora Blog

## Installation

Needs:
- `nodejs` and `npm`
- `docker`

```bash
$ npm i -g http-server gulp
$ git clone https://github.com/heiss-blog/antora.git
$ git clone https://github.com/heiss-blog/antora-ui-default.git
$ git clone https://github.com/heiss-blog/homepage.git
$ git clone https://github.com/heiss-blog/architecture.git
$ git clone https://github.com/heiss-blog/libraryinformationsystem.git
$ git clone https://github.com/heiss-blog/management.git
$ git clone https://github.com/heiss-blog/operatingsystems.git
$ git clone https://github.com/heiss-blog/productivity.git
$ git clone https://github.com/heiss-blog/softwaredevelopment.git
```

## Usage

```bash
$ gulp bundle -f antora-ui-default
$ docker run -v ${pwd}:/antora:Z antora/antora --cache-dir=./.cache/antora local-playbook.yml
$ # docker run -v ${pwd}:/antora:Z antora/antora --cache-dir=./.cache/antora antora-playbook.yml
$ http-server build/site -c-1
```
