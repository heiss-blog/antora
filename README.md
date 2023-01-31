# Antora Blog

## Installation

Needs:
- `nodejs` and `npm`
- `docker`

```bash
$ npm i -g http-server
```

## Usage

```bash
$ docker run -v ${pwd}:/antora:Z antora/antora --cache-dir=./.cache/antora antora-playbook.yml
$ http-server build/site -c-1
```
