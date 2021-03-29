copied from https://auth0.com/docs/flows

Authentication Authorization
Determines whether users are who they claim to be Determines what users can and cannot access
Challenges the user to validate credentials (for example, through passwords, answers to security questions, or facial recognition) Verifies whether access is allowed through policies and rules
Usually done before authorization Usually done after successful authentication
Generally, transmits info through an ID Token Generally, transmits info through an Access Token
Generally governed by the OpenID Connect (OIDC) protocol Generally governed by the OAuth 2.0 framework
Example: Employees in a company are required to authenticate through the network before accessing their company email Example: After an employee successfully authenticates, the system determines what information the employees are allowed to access

[<== Back](README.md)
