## Sample Application for Ionic Chat app using NodeJS Socket IO

## Easy to get started setup backend
- Step 1: click this => [![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/csantanapr/ionic-chat)
- Step 2: Enable CORS on the Cloudant Instance
- Step 3: Change permissions on **photos_db** database (read, write, replicate)

### To work locally with the code download source code via git or Download Zip button
```bash
    $ git clone https://github.com/csantanapr/ionic-chat
    $ cd ionic-chat
    $ npm install
```
    
### Run using Ionic on Mobile Device or Simulator

- Set the hostname of WebSocket server for Ionic App to connect. 
  - Edit `www/js/app.js`, change from http://ionic.mybluemix.net to your local ip or remote host on Bluemix after deploying app.
  - Edit `www/js/app.js`, change __DBUrl__ with your own couchdb/cloudant DB
  - Run `$ ionic prepare` after making the change
  
```bash
    $ ionic platform add ios
    $ ionic platform add android
    $ ionic run android
    $ open platforms/ios/*.xcodeproj
```

### Run the NodeJS Chat Server locally
```bash
    $ npm start
    $ open http://localhost:8080
```

### Run simple Websockets demo
```bash
    $ cd simple_websocket
    $ npm install
    $ npm start
    open browser on http://localhost:6001
```

### Run simple Socketio demo
```bash
    $ cd simple_socketio
    $ npm install
    $ npm start
    open browser on http://localhost:6001
```
  
  
### Software Requirements:
- Minimum
  - [Bluemix Free Account](https://console.ng.bluemix.net/registration)
  - Mobile or Desktop Browser with WebSockets support (http://caniuse.com/#feat=websockets)	
- To run local Server
  - NodeJS: Install via [nvm](https://github.com/creationix/nvm) or [nodejs.org](https://nodejs.org/en/download)
- To run on Mobile Simulator or Device
  - Install Ionic and Cordova CLI
	  - npm install -g ionic cordova  (you might need to use sudo)
  - Android 
    - Java SDK (setup PATH, test javac on terminal)
    - Android SDK (setup PATH, test android and adb on terminal)
  - XCode and XCode Commad Tools (test xcode-select -p and xcodebuild)
	
#### License: [Apache 2.0](License.txt)
