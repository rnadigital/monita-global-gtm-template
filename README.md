# Monita Global Monitoring

Google Tag Manager tag template for Monita global monitoring. One tag loads the
Monita script for a property and reports every vendor event on the page, with
the container ID and version attached.

## Set up

1. Add a website property in Monita and copy its token (starts with `dom_`).
2. In GTM, add a tag of type **Monita Global Monitoring** from the Community
   Template Gallery and paste the token.
3. Fire it on **Initialization - All Pages**, preview, then publish.

**Script host** picks where the script loads from: `cdn.monita.ai` (default) or
the legacy `cdn-a.raptor.digital`. Both serve the same script. Events always go
to the collection endpoint set on the property in Monita, including your own
first-party hostname when one is configured, whichever host loads the script.

Docs: https://docs.monita.ai/install/websites/
