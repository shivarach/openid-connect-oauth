# openid-connect-oauth

## OAuth 2.0 terminology
Assume the scenario an application 'x' wants to access your google contacts to send an invitation

* Resource owner: User who owns data
* Client: The appliction which wants access to some data i.e. x
* Authorization server: server to which user says yes to give grants to the client Eg: google accounts server
* Resource server: the actual data server eg:google contacts (some times authorization and resource servers are same)
* Authorization grant: authorization grant code
* Redirect URI: callback to the client 'x'
* Access token: client 'x' gets a token which indicates what resources x can access
* scope: the scope(define in authorization server) which limits the grant level
* consent:the screen where user says yes/no


Some network terminology:
* back channel: calling a server from our own backend server (more secured)
* front channel: calling a server from browser(less secured since it can seen in chrom debug tools)

** OAuth 2.0 flows
* Authorization code (front channel + back channel) - recommended
* Implicit (front channel only) - single page applications
* Resource owner password credentials(back channel only)
* Client credentials (back channel only)


## OpenID Connect
oAuth is meant for authorization but it is overused as an authentication also but it is a hack. So to make it better **openid connect** came into picture. The openid connect is just 5% wrapper on top of oAuth which can be used for authentication.


### OpenID connect adds
* ID token (user identification)
* Userinfo endpoint for getting more user info
* Standard set of scopes
* Standardized implementation
