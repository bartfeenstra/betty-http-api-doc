
# HTTP API Documentation for Betty 👵

![Test status](https://github.com/bartfeenstra/betty-http-api-doc/workflows/Test/badge.svg) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty-http-api-doc/branch/master/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty-http-api-doc) [![PyPI releases](https://badge.fury.io/py/betty-http-api-doc.svg)](https://pypi.org/project/betty-http-api-doc/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty-http-api-doc.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty-http-api-doc/) [![Recent downloads](https://img.shields.io/pypi/dm/betty-http-api-doc.svg)](https://pypi.org/project/betty-http-api-doc/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project) 

[Betty](https://pypi.org/project/betty/) is a static site generator for your [Gramps](https://gramps-project.org/) and
[GEDCOM](https://en.wikipedia.org/wiki/GEDCOM) family trees.

*HTTP API Documentation for Betty* is a Betty extension that renders interactive and user-friendly HTTP API documentation using
[ReDoc](https://github.com/Redocly/redoc).

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Contributions](#contributions)
- [License](#license)

## Installation

### Requirements
- **Python 3.7+**
- Node.js 10+
- Linux, Mac OS, or Windows

### Instructions
Run `pip install betty-http-api-doc` to install the latest stable release.

To install the latest development version, run `pip install git+https://github.com/bartfeenstra/betty-http-api-doc.git`. If you
want the latest source code, read the [development](#development) documentation.

## Usage
This extension can be enabled through Betty's GUI, or by adding the following to your Betty configuration file:
```yaml
extensions:
  betty_http_api_doc.extension.HtpApiDoc: ~
```

## Development
First, [fork and clone](https://guides.github.com/activities/forking/) the repository, and navigate to its root directory.

### Requirements
- The installation requirements documented earlier.
- Bash (you're all good if `which bash` outputs a path in your terminal)

### Installation
In any existing Python environment, run `./bin/build-dev`.

### Working on translations
To add a new translation, run `./bin/init-translation $locale` where `$locale` is a
[IETF BCP 47](https://tools.ietf.org/html/bcp47), but using underscores instead of dashes (`nl_NL` instead of `nl-NL`).

After making changes to the translatable strings in the source code, run `./bin/extract-translatables`.

### Testing
In any existing Python environment, run `./bin/test`.

### Fixing problems automatically
In any existing Python environment, run `./bin/fix`.

## Contributions 🥳
HTTP API Documentation for Betty is Free and Open Source Software. As such you are welcome to
[report bugs](https://github.com/bartfeenstra/betty-http-api-doc/issues) or
[submit improvements](https://github.com/bartfeenstra/betty-http-api-doc/pulls).

## Copyright & license
HTTP API Documentation for Betty is copyright [Bart Feenstra](https://twitter.com/BartFeenstra/) and contributors, and released under the
[GNU General Public License, Version 3](./LICENSE.txt). In short, that means **you are free to use HTTP API Documentation for Betty**,
but **if you distribute HTTP API Documentation for Betty yourself, you must do so under the exact same license**, provide that license, 
and make your source code available.
