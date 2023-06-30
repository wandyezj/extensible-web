# Components

The overall architecture is that a host site loads extensions in separate iframes to maintain a security boundary.

The host site loads the [Extension Host](#extension-host) and can then use that host to load extensions in individual iframes.

An extension is loaded in an iframe and then loads the [Extension Client](#extension-client) which establishes the connection to the host.

The extension client can then ask the host for the APIs available and populates these APIs.

The versions of the extension client and extension host needs to match or be compatible.

## Extension Host

A host website loads the extension host which can then load extensions.

The extension host handles API requests from loaded extensions and responds with the appropriate data.

A host website can have different ways to keep track of which extensions should be loaded. These could be hard coded or loaded on demand based on user preferences.

The extension host is a generic package that does not change between sites.

## Extension Client

The extension client is loaded by an extension and connects to the extension host.

The extension client populates itself with the APIs available from the host.

The extension client handles API requests from the extension and responds with the appropriate data.

The extension client is a generic package that does not change between sites.

## API

APIs are how an extension can interact with the host website.

API should be thought of as a strict contract between the host and the extension.
