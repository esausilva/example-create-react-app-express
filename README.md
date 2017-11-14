# create-react-app React Project with Node Express Backend

> Example on using create-react-app with a Node Express Backend

## Usage

Install [nodemon](https://github.com/remy/nodemon) globally

```
npm i nodemon -g
```

Install server and client dependencies

```
yarn
cd client
yarn
```

To start the server and client at the same time

```
yarn dev
```

## How this works

The key to use an Express backend with a project created with `create-react-app` is on using a **proxy**. We have a *proxy* entry in `client/package.json`

``` 
"proxy": "http://localhost:5000/"
```

This tells Webpack development server to proxy our API requests to our API server, given that our Express server is running on **localhost:5000**

-Esau
