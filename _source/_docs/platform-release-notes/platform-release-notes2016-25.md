---
layout: docs_page
title: Platform Release Notes June 22, 2016
---

# Release 2016.25

## New Platform Feature: Limit on Size of Groups Claim
    
To protect against arbitrarily large numbers of groups matching the group filter, the group claim has a limit of 100. 
If more than 100 groups match the filter, then the request fails.

* For more information about configuring an app for OpenID Connect, including group claims, see [Using OpenID Connect](). 
* For more information about group claims in the API, see [Scope-dependent claims](/standards/OIDC/index.html#scope-dependent-claims-not-always-returned).

## Bugs Fixed

The following issues are fixed:

* OKTA-89624 – Base schema attributes for OpenID Connect without default mappings weren't included in ID token claims.
* OKTA-89867 – Creating a new user and adding that user to a group with the same create request via the API failed, which was a problem for group-scoped User Admins creating users.
* OKTA-90593 – The Group property <em>lastMembershipUpdated</em> wasn't updated when adding or removing users from an Active Directory group using scheduled import.
* OKTA-90898 – Updating credentials failed when using the Apps API for custom apps.
* OKTA-91066 – System log messages related to OpenID Connect didn't contain scopes.

Added on June 29: 

* OKTA-90514 – When adding a group target to a User Admin role via the API, that user still had the ability to administer all groups. Also, removing the last group target from a role after one has been added was incorrectly allowed.

## Looking for Product Release Notes?

For changes outside the Okta platform, see the [Release Notes Knowledge Hub](https://support.okta.com/help/articles/Knowledge_Article/Release-Notes-Knowledge-Hub).

## Return to Current Release Notes

[Current Platform Release Notes](platform-release-notes.html)
