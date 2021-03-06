# MSAL Angular Public APIs for MSAL Angular v2

Before you start here, make sure you understand how to [initialize the application object](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/msal-angular-v2/lib/msal-angular/docs/v2-docs/initialization.md).

The login APIs in MSAL retrieve an `authorization code` which can be exchanged for an [ID token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens) for a signed in user, while consenting scopes for an additional resource, and an [access token](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) containing the user consented scopes to allow your app to securely call the API.

You can read more about ID tokens on our [Azure Docs pages](https://docs.microsoft.com/azure/active-directory/develop/id-tokens).

## Public APIs

MSAL Angular exposes the following, along with their configurations 
1. [`MsalService`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/msal.service.ts/)
2. [`MsalGuard`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/msal.guard.ts/)
    * [`MsalGuardConfiguration`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/msal.guard.config.ts/)
3. [`MsalInterceptor`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/msal.interceptor.ts/)
    * [`MsalInterceptorConfiguration`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/msal.interceptor.config.ts/)
4. [`MsalBroadcastService`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/msal.broadcast.service.ts/)
5. [`MsalModule`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/msal.module.ts/)

The login and acquire token functions using Angular observables are found on the [IMsalService](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-angular/src/IMsalService.ts/).

Additional functions from `@azure/msal-browser` are found on [`IPublicClientApplication`](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/src/app/IPublicClientApplication.ts), with corresponding documentation [here](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/login-user.md).
