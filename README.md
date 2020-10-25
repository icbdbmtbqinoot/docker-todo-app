# docker-todo-app
This project was created with [Docker Labs](https://dockerlabs.collabnix.com/)

## Available Scripts

Build a container image by running:

### `docker build -t <image tag name> .`

Start an app container by running:

### `docker run -dp 3000:3000 <image tag name> .`

Open [http://localhost:3000](http://localhost:3000) to view it in the browser

Start an app with developer mode:

### `docker run -dp 3000:3000 \
    -w /app -v "$(pwd):/app" \ 
    node:12-alpine \ 
    sh -c "yarn install && yarn run dev".`
    
Open [http://localhost:3000](http://localhost:3000) to view it in the browser
The page will reload if you make edits.<br />

To persist data using MySQL
Start up the application stack by running:

### `docker-compose up -d`

Open [http://localhost:3000](http://localhost:3000) to view it in the browser
