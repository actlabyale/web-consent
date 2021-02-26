Test URL: https://actlabyale.github.io/web-consent/sona-30/?dest=https://github.com/sdmcdougle&tab=repositories&prolific=1&id=100

(current subdirs are `sona-30`, `sona-60`, and `prolific`)
The general idea is that when we post a study on Prolific/MTurk/etc, we would set the URL to be of the form:

```
https://actlabyale.github.io/web-consent/<consent type>/?dest=<interesting URL>
```

Make sure that any parameters are specified in the Prolific dialog (e.g. `&group=b`), not as part of the experiment URL (e.g. `https://actlabyale.github.io/web-consent/sona-30/?dest=https://github.com/sdmcdougle&tab=1&prolific=1` is difficult to parse?).

Additional parameters added by the service (i.e. the participant number) _should_ be added properly to the end (see e.g. `&id=100` above).

Note that we need a polyfill to allow URL parsing for Internet Explorer.

The duration of time spent on the consent form is recorded as `consentTime` in the URL.
