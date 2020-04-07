# JOSN Server
This is a temporary server that provide basic api to read and write to json file using local server.

## How to run
There are several step that you need to follow in order to make it working

* Install all the dependencies mentioned in package.json file
```bash
> npm install
```

* Run json server on port 3000 if not occupied
```bash
# Change the db script in package json if port 3000 is occupied
# "db": "json-server -w db.json -p 3001"
# Then run the following command
> npm run db
```

* Create a tunnel that will allow multiple devices to interact with your local server. Open new terminal/console window
```bash
# After running the following command, use "Forwarding" url with the patter "http://<xxxxxxx>.ngrok.io" in your application.
# This will point to the http://localhost:3000 on your system. 
# Change the port in tunnel script if you changes the port of json-server

> npm run tunnel
```
**NOTE**: This tunnel url will only be available around 8 hours. you need to terminate tunnel and re-run the command in order to acquire new forwarding url that you will again be available for 8 hours.

