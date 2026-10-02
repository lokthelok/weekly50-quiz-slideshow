# weekly50-quiz-slideshow
slideshow type rendering of the Weekly50 quiz

## Corsfix Setup

Quiz requests use the Corsfix SDK, which is required for free production access, with domain whitelisting rather than an API key. Add the site's domain (`lokthelok.github.io`, origin `https://lokthelok.github.io`) to your application in the [Corsfix dashboard](https://app.corsfix.com/). The browser supplies the Origin header automatically.

The [free production tier](https://corsfix.com/docs/free-tier) allows one concurrent user and 10 MB monthly transfer per domain, increasing to 100 MB for a registered application. Requests fail when limits are reached; the SDK displays a dismissable notice.

Serve local previews over HTTP rather than opening a `file:` URL. Local preview access is subject to Corsfix's development-domain policy and your account configuration. The production domain must be enabled before the deployed slideshow can load the quiz.
