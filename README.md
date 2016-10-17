Docker Hub CLI
========
[![PyPI version](https://badge.fury.io/py/docker-hub.svg)](https://badge.fury.io/py/docker-hub)

[![asciicast](https://asciinema.org/a/88278.png)](https://asciinema.org/a/88278)

A CLI tool to access Docker Hub from your terminal.

## Installation
You should have pip installed in your system.
```sh
pip install docker-hub
```
python 3 users can do
```sh
pip3 install docker-hub
```

## Usage
##### 1. Authenticate with Docker Hub
If you are already loggedin using `docker login` command, then the token in docker engine config will be used. Otherwise you will be prompted to enter username and password. 

##### 2. Querying an organization for repositories
To query repositories in an organization use `repos` argument. The organization to query can be passed as `--orgname` parameter.  
eg: Get repos in organization named "docker"
```sh
docker-hub repos --orgname=docker
```

##### Notes:
Only 15 results for any query are displayed at once. You can fetch remaning pages by passing `--page` parameter. 

eg: Get 3rd page
```sh
docker-hub repos --orgname=docker --page=3
```

## Development
Questions, problems or suggestions? Please post them on the [issue tracker](https://github.com/amalfra/docker-hub/issues).

You can contribute changes by forking the project and submitting a pull request. Feel free to contribute :heart_eyes:

UNDER MIT LICENSE
=================
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
