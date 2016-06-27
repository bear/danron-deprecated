[![Downloads](https://img.shields.io/pypi/v/danron.svg)](https://pypi.python.org/pypi/danron/)
[![Requirements Status](https://requires.io/github/bear/danron/requirements.svg?branch=master)](https://requires.io/github/bear/danron/requirements/?branch=master)
[![codecov](https://codecov.io/gh/bear/danron/branch/master/graph/badge.svg)](https://codecov.io/gh/bear/danron)

談論 - discussion

Danron is a Python Flask app designed to facilitate distributed [IndieWeb](https://indiewebcamp.com) Chat.

## Requirements and Assumptions
- Python v2.7
- Danron is written using Flask and takes advantage of the builtin Jinja template handling
- Because Danron needs to to store state information for authentication and authorization, it requires a Redis database
- All Micropub and Webmention calls are handled, dispatched and then an HTTP code 202 is returned.

## Configuration

The Flask part of Danron uses the normal Flask ```settings.py``` configuration file, see https://github.com/bear/Danron/blob/master/Danron/settings.py for reference.

## Installation
All of the dependencies are outlined in a pip installable ```requirements.txt``` file.

## Running

dev mode - ```make server```

uwsgi - ```make uwsgi```


## Todo
- allow micropub create
- allow webmentions ala brid.gy publish
 - scan sourceurl for a single chat/note
 - scan sourceurl for all chat/notes, cache?
- push
- pubsubhubbub
- superfeedr
