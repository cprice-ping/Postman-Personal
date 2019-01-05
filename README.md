# Postman-Personal
Collections I'm working on - those of interest to the broader Ping Identity audience will be moved over to the Ping Repository

Those posted here are not all in a finished state - but could be used to start working with Ping Identity APIs.

Many of these are being used to Train \ Attack the API endpoints protected by PingIntelligence - they are designed to be self-contained in Postman Collection Runner iterations. Collections used in this way will have a "Training" and "Attack" Folder in them.

## Collection - Consent API

This Collection is built to:

* Demonstrate the Consent API in PingDirectory
* Train PingIntelligence with appropriate calls
* Attack PingIntelligence with inappropriate calls

The "Training" folder contains calls that show correct usage of the API

*Notes*: 

Consent Definitions need to be created in PingDirectory Admin Console first

Some calls contain hardcoded mapping of Definitions to Audience. If you want to use this against your own instance of Consent API, the array is held in Collection Variables

## Collection - PingFed Admin API

This set demonstrates the new APIs in PF 9.2+ that allow you do use the Admin API to fully build out a PingFed server that's connected to PingDirectory.

This set of calls:
* Accepts EULA
* Imports a PingFed license (stored in the Environment)
* Adds the intitial Admin user
* Enables the Server Roles
* Adds PingDirectory as a Data Store
* Adds a LDAP Password Credential Validator
* Adds a HTML Form Adapter with the PCV
* Adds an AuthN Policy with Contract
