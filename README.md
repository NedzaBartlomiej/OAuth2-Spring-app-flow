![OAuth2WithSpringAppFlow](https://github.com/NedzaBartlomiej/OAuth2-Spring-app-flow/assets/86315326/46e7e251-d197-4f6b-bbd7-54243954d67f)

### Getting token (Access Token/ID Token) from Google
1. When resource-owner login correctly on Google login page, the `Authorization Code` is returned to client
2. Client requesting for token with `Authorization Code` (to auth-server)
3. The token is returned to client
4. And used in requests to resource-server.


### Access Token vs ID Token 
##### Access Token:
- is used for auth to something resource (for example: for Google Calendar API, u can access with it for e.g. user's task, event or something else that Google providing in API)

##### ID Token:
- is used for identify the user (contains the OpenId, thanks to which you can f.e integrate your db user with Google identified user from token), it can also contains something identification data/informations, like email, username or something else.
