# honeyishrunktheurl-html

A completely client-side URL shortener. Written in HTML and client-side JavaScript.


## Requirements

You need a server.

Use Nginx/Apache in production, but for local development any basic server will do. (Stay away from Python's `SimpleHTTPServer` because of [this bug/feature](http://bugs.python.org/issue17324). Use [`http-server`](https://www.npmjs.org/package/http-server) instead:

	npm install http-server -g && http-server


## Usage

1. Copy over a `sites.js`:

        cp sites.js{.dist,}

    This is where your routes live.
2. Have your server route all root-level traffic (`/.*`) to `/index.html`.
3. Load [http://localhost:8080/cvan](http://localhost:8080/cvan). (Or if you haven't rewritten the URLs, simply load [http://localhost:8080/?cvan](http://localhost:8080/?cvan).)
