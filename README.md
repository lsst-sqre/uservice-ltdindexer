[![Build Status](https://travis-ci.org/lsst-sqre/uservice-ltdindexer.svg?branch=master)](https://travis-ci.org/lsst-sqre/uservice-ltdindexer)

# sqre-uservice-ltdindexer

LSST DM SQuaRE api.lsst.codes-compliant microservice wrapper to provide an
LSST The Docs index page.

## Usage

`sqre-uservice-ltdindexer` will run standalone on port
5000 or under `uwsgi`.  It responds to the following routes:

### Routes

* `/`: returns `OK` (used by Google Container Engine Ingress healthcheck)

* `/ltdindexer`, `/ltdindexer/json`: returns JSON structure with two
  fields: `ul`, which contains a UTF-8-encoded HTML ul entity
  with the list of documents on LTD, and `index`, which contains a
  UTF-8 encoded HTML document wrapping the document list.

* `/ltdindexer/page`: returns the index page (not as JSON).
