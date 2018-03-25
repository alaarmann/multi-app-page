This site is trying to evolve the idea of a __multi-app page (MAP)__, a concept where the user has control over what applications to use on a web page and what data to share.

It conveys the opinionated view of the author(s). As a work in progress it can undergo changes at any time. The changes are reflected transparently by the backing GitHub repository [alaarmann/multi-app-page](https://github.com/alaarmann/multi-app-page/).

## Challenge

When a user loads a web page in her browser, it is quite common that the page in turn loads further JavaScript applications from other domains and other owners. If these applications are somewhat independent from the page and have a value of their own (e.g. a chat client), we could call that web page a _multi-app page_.

We see the following shortcomings here:
- The owner of the web page decides what applications her page offers to the user. She may leave a choice to the user, but only out of a pre-restricted set.
- If no additional measures are taken, all applications and their owners have full access to the web page's data (e.g. URI, cookies, content). It is common case that the web page contains also the users private data, that is hence put at stake without her knowledge.

For us this poses the challenge to create an intermediate entity that enables the user to add whatever application she wants to the page and that lets her transparently control whether this application should be given access to the pages data and to what extent.


## Vision

We advocate the concept of a multi-app page (MAP) as follows:

A user working with a MAP has the option to add one or more applications of her free choice to the page and control their access to the page's data.

By default, such an application is completely isolated from the page and has no access to anything outside itself. This is already sufficient for applications that function fully independently. The user wants to have the application on the page for faster access or immediate notification while she is using the page.

The great potential however lies in the interaction between the application and the page. To that end the user can explicitly permit the application to access the page's data and/or pass its own data to the page. That opens up the page for value-added functions to the benefit of the user. Such functions are able to enrich the page in ways not even foreseen by the page owner.

The user has full transparency over the extent of interaction between application and page and can revoke her permission to interact at any time or even disable the use of the application completely.

The page owner for her part has the guarantee that the application will not have a negative impact on the functioning of her page, e.g. breaking functions or corrupting content.

## Example

## Implementation
### Isolation
### Interaction
### Trust

TLS-secured URL


## Bigger Picture

Environment: Operating System
Up to now cross-application interaction in the frontend is only poorly supported. The common way to exchange data between user-facing applications is to _copy_ it to the 'clipboard' and _paste_ it in the destination. Type of data, mismatch, poor integration of apps.

New: environment browser
 Runtime environment for always 'heavier' frontend applications, rise of SPA, advent of WebAssembly.
 Semantic markup, microformats make it possible to exchange 'typed' information with semantic value.

Never trust the server: shift the linking between systems to the frontend. Give the user more control over inter-connections between systems.

## Comparison to related concepts

## Maintainer
This site is maintained by [@alaarmann](https://twitter.com/alaarmann) and hosted by GitHub Pages. The backing repository can be found at [alaarmann/multi-app-page](https://github.com/alaarmann/multi-app-page/).
