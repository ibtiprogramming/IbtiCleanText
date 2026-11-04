# Privacy notes

The current CleanText implementation performs text processing in the browser using the JavaScript contained in `index.html`. It does not include an account system or a server-side text-processing endpoint.

Because this is a static browser app, text you enter is processed by the page in your browser. Avoid adding analytics, remote logging, or third-party processing without clearly documenting the change and its privacy implications.

This note describes the current source code; hosting providers may still collect ordinary website access logs when the page is published online.
