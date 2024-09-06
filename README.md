Repository for fake JWKS endpoints for using to test CIS2. 

Only used when we can't allow NHS access to our server to directly talk to us. 

To create a listing for your server set up the CIS2 jks cert store on the server and go to:
{myServer}/nhs-auth-response/jwks.json

Copy the content of the file into a new .json file and upload it to the repo. 

Suggest logically ordering things into folder for NHS environemt (should only be INT really) and then a folder for the server

If you update the certs you'll need to update the content of the json file on here 

The URL given to NHS should be the raw version of the file (navigate to the file on github and click raw) url will be like:
https://raw.githubusercontent.com/nervecentresoftware/CIS2-JWKS/main/{ENVIRONMENT NAME}/{SERVER NAME}/jwks.json
