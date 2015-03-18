# Non `www`-prefixed redirector

Simple redirector for non `www`-prefixed domains.

## Why?

Built for the [ThoughtJot!](https://github.com/roberthodgen/thought-jot) project, this will redirect users to the `www`-prefixed domain.

Google App Engine will not serve SSL/secure on a naked domain. This project is served at the naked domain redirecting to the `www`-prefixed equavilent.

## Example

A user requests `http://thoughtjot.net/projects`, they are redirected (via this project) to `http://www.thoughtjot.net/projects` (the `www`-prefixed equavilent).

_Note: the [ThoughtJot! `app.yaml` file](https://github.com/roberthodgen/thought-jot/blob/master/src/app.yaml) redirects to secure pages.__

## How to use it

1. Create a Project with any name.
2. In `app.yaml`, set the `application: *your-app-id*` to your project's name.
3. Point your naked domain to the project.

Enjoy :)
