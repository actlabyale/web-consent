The general idea is that when we post a study on Prolific/MTurk/etc, we would set the URL to be of the form:

```
https://actlabyale.github.io/web-consent?dest=<interesting URL>
```

e.g.

```
https://actlabyale.github.io/web-consent?dest=https%3A%2F%2Fgithub.com%2Fsdmcdougle%3Ftab%3Drepositories&id=100
```

(sort of annoying thing right now-- need to pass the experiment URL through `encodeURIComponent` so that the link passes everything properly).

Additional parameters added by the service (i.e. the participant number) _should_ be added properly to the end (see e.g. `&id=100` above).

TODO: Update consent to latest!
