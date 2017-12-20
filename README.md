# Simple docker container for a simple node js http app
- one container from `node:carbon` 
- command to run on start in the compose file (because I am not using my own `Dockerfile`)
- the container opens port 8080 and maps it to 8080 (which the node script is listening to)
- one `server.js` file is called in the `package.json` startup script
- the `server.js` creates an http server which listens to port 8080 and returns text and http code `200`