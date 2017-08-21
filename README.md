# GitHub Connector 
This contains the source for the GitHub connector for Microsoft Teams.
 
#### Prerequisites
1. Register a new OAuth application at GitHub. Note the GitHub client id and secret.
2. Download ngrok from https://ngrok.com/. Run the following command to setup a tunnel to localhost:3000
 `ngrok http 3000`
 Note the ngrok address, which looks something like `https://013e0d3f.ngrok.io`.
3. Put the callback Url in the Oauth app as 'your-ngrok/auth/github/callback'.
4. Replace the clientId,clientSecret,callbackUrl and serviceUrl in Default.json.

### Configuration 
 - Default configuration is in `config\default.json`
 
### How to Run
 - install all the dependencies through npm install.
 - run node server.js.
 - Zip manifest.json file and sideload to any team. Alternative you can set your own connector at Microsoft connector portal (https://outlook.office.com/connectors/publish) and follow instructions here to get a new connector for microsoft teams ( https://msdn.microsoft.com/en-us/microsoft-teams/connectors).
