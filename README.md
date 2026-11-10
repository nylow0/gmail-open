# gmail-open

A one-file redirect page used by a private email digest bot. A digest link like
`https://nylow0.github.io/gmail-open/#a=<account>&m=<message id>` opens that email:
the Gmail app on Android, Gmail web elsewhere.

- Data lives in the `#fragment`, which browsers never send to this server.
- The page only ever navigates to `mail.google.com` / the Gmail app and rejects anything else (no open redirect).
- No data, no tracking, no external resources; strict Content-Security-Policy.

Source and tests live in a private repo; this copy is published from there.
