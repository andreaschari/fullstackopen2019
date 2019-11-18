browser->server HTTP GET https://fullstack-exampleapp.herokuapp.com/spa

server->browser server sends html code

browser->server: HTTP GET https://fullstack-exampleapp.herokuapp.com/main.css to get CSS Style sheet

server-->browser: server sends main.css 

browser->server: HTTP GET https://fullstack-exampleapp.herokuapp.com/spa.js to get JavaScript code

server-->browser: server sends spa.js

browser runs js code requesting  JSON data from the server

browser->server: HTTP GET https://fullstack-exampleapp.herokuapp.com/data.json to get the JSON data

server-->browser server sends JSON data

browser executes event handler and renders list