Test URL: https://actlabyale.github.io/web-consent?dest=https://github.com/sdmcdougle&tab=1&prolific=1

The general idea is that when we post a study on Prolific/MTurk/etc, we would set the URL to be of the form:

```
https://actlabyale.github.io/web-consent?dest=<interesting URL>
```

e.g.

```
https://actlabyale.github.io/web-consent?dest=https://github.com/sdmcdougle&prolific=1
```

Make sure that any parameters are specified in the Prolific dialog (e.g. `&group=b`), not as part of the experiment URL (e.g. `https://actlabyale.github.io/web-consent?dest=https://github.com/sdmcdougle&tab=1&prolific=1` is difficult to parse?)

Additional parameters added by the service (i.e. the participant number) _should_ be added properly to the end (see e.g. `&id=100` above).

Note that we need a polyfill to allow URL parsing for Internet Explorer.

TODO: Update consent to latest!
