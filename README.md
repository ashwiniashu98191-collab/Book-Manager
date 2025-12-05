# Book-Manager

A web application for managing a library or collection of books using their ISBNs as references.

# Steps to run

used a web server(ubuntu)

## Clone the repository

git clone https://github.com/emurenMRz/book-manager

cd book-manager

## Run the App

docker compose build(# Build the base image)

docker compose run --rm web rake db:create db:migrate

docker compose run --no-deps web rails new . --force --database=postgresql --skip-test(Run Rails generator inside web container)

docker compose up

## Visit the app at

http://localhost:8000
