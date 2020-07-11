# short-url
### Description
This is a tiny demo app that uses Vue.js on the client (served via nginx) and Express/MongoDB on the server.

### Installation:
```sh
$ git clone --recurse-submodules git@github.com:danielcaballero/short-url.git
$ cd short-url
$ docker-compose build
$ docker-compose up
```
Then you can open your browser at `http://localhost:8001`

### Specs:
The app meets the following requirements:
- A user needs to be able to enter a URL and they will get an 8 character (lowercase-alphanumeric) shortened version of the URL.
- URLs are shortened and persisted into MongoDB via a REST API.
- The frontend app will display a list of previously shortened URLs.
- New URLs will be generated and added to the frontend list.
- The same 8-characters cannot be used twice i.e. each shortened URL needs to be unique.
- The URLs need to be shortened with the following domain 'pbid.io' e.g. https://pbid.io/f3x2ab1c
- The shortened URL do not need to actually redirect/work as the domain doesn’t exist.
- The entire system needs to be runnable using Docker, a simple compose file will do.
- Appropriate tests should be added to the code, using the jest framework.
- The app layout should be responsive.
