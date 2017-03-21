[![Build Status](https://travis-ci.org/lsst-sqre/uservice-ltdindexer.svg?branch=master)](https://travis-ci.org/lsst-sqre/uservice-ltdindexer)

# sqre-uservice-ltdindexer

LSST DM SQuaRE api.lsst.codes-compliant microservice wrapper.  TODO

## Usage

`sqre-uservice-ltdindexer` will run standalone on port
5000 or under `uwsgi`.  It responds to the following routes:

### Routes

* `/`: returns `OK` (used by Google Container Engine Ingress healthcheck)

* `/ltdindexer`: TODO

### Returned Structure

The returned structure is JSON.  TODO.
