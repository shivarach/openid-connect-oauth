# openid-connect-oauth

## OAuth 2.0 terminology
Assume the scenario an application 'x' wants to access your google contacts to send an invitation

* Resource owner: User who owns data
* Client: The appliction which wants access to some data i.e. x
* Authorization server: server to which user says yes to give grants to the client Eg: google accounts server
* Resource server: the actual data server eg:google contacts (some times authorization and resource servers are same)
* Authorization grant: point where user clicks yes/no to give data(contacts)
* Redirect URI: callback to the client 'x'
* Access token: client 'x' gets a token which indicates what resources x can access
