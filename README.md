# verona

Where the environments live.

`verona` is the private configuration for
[romeu e julieta](https://github.com/brunovenceslau/romeu-e-julieta): it
describes every development project, and `romeu` turns those
descriptions into a deterministic tree on the host, one sandbox per
project, with `julieta` working inside each sandbox.

## What lives here

```
verona/
├─ projects/
│  └─ <name>.yaml    one file per project: its repositories, kits,
│                    sandbox options, secret names and run layout
└─ kits/
   └─ <name>/        personal kits, composed into a project's sandbox
```

Secrets never live here: a project names the secrets it needs, and the
host configuration alone decides how each one is resolved.

## Status

Empty. The project spec format is being defined in romeu e julieta.
