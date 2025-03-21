# OAUTH Client Assertions

Three applications are using in this setup, an API which uses the access token, an OAuth client application implemented as a console app and a OAuth server, implemented using ASP.NET Core and Duende IdentityServer. OAuth client credentials is used to acquire the access token and the signed JWT is used to authenticate the client request.

> Note
> 
> Code created from the Duende samples and Duende IdentityServer

![flow](https://github.com/damienbod/OAuthClientAssertions/blob/main/images/OAuthCCSignedJWTAssertion.png)

## Migrations

```
Add-Migration "InitializeApp" -Context ApplicationDbContext
```

```
Update-Database -Context ApplicationDbContext
```

## Links

https://docs.duendesoftware.com/identityserver/v7/tokens/authentication/jwt/

https://docs.duendesoftware.com/identityserver/v7/reference/validators/custom_token_request_validator/

https://docs.duendesoftware.com/identityserver/v7/tokens/authentication/jwt/

https://docs.duendesoftware.com/foss/accesstokenmanagement/advanced/client_assertions/

https://www.scottbrady.io/oauth/removing-shared-secrets-for-oauth-client-authentication

https://damienbod.com/2025/02/24/use-client-assertions-in-openid-connect-and-asp-net-core/
