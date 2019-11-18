browser->server HTTP POST https://fullstack-exampleapp.herokuapp.com/new_note

browser sends the new note to the server

server->browser server responds with code 302 and causing a redirect

browser->server HTTP GET to header location i.e. /notes

browser reloads page causing three more requests

browser->server HTTP GET https://fullstack-exampleapp.herokuapp.com/main.css to get the CSS stylesheet

server->browser server sends main.css

browser->server HTTP GET https://fullstack-exampleapp.herokuapp.com/main.js to get JavaScript code

server->browser server sends main.js

browser executes main.js that requests JSON data from the server

browser->server HTTP GET https://fullstack-exampleapp.herokuapp.com/data.json

server->browser server sends data.json

browser executes event handler and re-renders list with new note