# Sequences

## Host Extension Load

1. host website loads the extension host.
1. host website configures the extension host with available APIs and other settings.
1. host website loads extensions

## Extension Load

1. extension loads the extension client.
1. extension client connects to the extension host and requests metadata about the host {version, APIs, etc...}
1. extension client populates itself with the available APIs.
1. extension client signals to the extension that it is ready to be used.

## Extension API Call

(Assumes that extension has been loaded)

note: by design all API calls are asynchronous.

1. extension calls an API
1. extension client receives the API call and forwards it to the extension host.
1. extension host handles the API call and returns the result to the extension client.
1. extension client receives the result and returns it to the extension.

