# Under Construction :construction:

####This is a demo website to test and showcase the ["Sphereon Self Issued OpenID Provider v2 (SIOP)" library](https://github.com/Sphereon-Opensource/did-auth-siop) 


### Getting started

#### Configure environment
In the onto-demo-server folder, create a files called .env.local and populate it using .env as example.
A valid config will look like this
```dotenv
NODE_ENV=development
PORT=5001
COOKIE_SIGNING_KEY=8E5er6YyAO6dIrDTm7BXYWsafBSLxzjb
REDIRECT_URL_BASE=http://192.168.1.200:5001/ext
RP_DID=did:ethr:0xe1dB95357A4258b33A994Fa8cBA5FdC6bd70011D
RP_PRIVATE_HEX_KEY=850e54b92c6291a1ff7b8c3ef30e032571ed77c9e5c78b1cd6ee5fec4fea984f
AUTH_REQUEST_EXPIRES_AFTER_SEC=300
MOCK_AUTH_RESPONSE=false
```
(Exception for the IP address this is a valid configuration to test with.)


#### Build & start
From the root directory
- yarn global add concurrently
- yarn global add ts-node
- yarn install-all
- yarn build-types
- yarn start

The server will start on port 5001, the client will start & open a browser on http://localhost:3000/

#### Usage
Once the demo site has loaded, click "Sign in"
A QR code will appear which can be scanned with the mobile authenticator app "[rn-did-siop-example-app](https://github.com/Sphereon-OpenSource/rn-did-siop-example-app)"
After a successful login two extra page will appear in the menu navigation. 


