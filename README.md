# kryptowithk.github.io

GitHub Pages user site (domain root for the project sites under kryptowithk.github.io/*).

It exists only to serve Square's Apple Pay domain verification file at
`/.well-known/apple-developer-merchantid-domain-association`, so Apple Pay (via Square Web Payments SDK)
works on https://kryptowithk.github.io/convenience-liquors-preview/checkout/.

* `.nojekyll` is required: without it GitHub Pages (Jekyll) skips dot-folders like `.well-known`.
* The file comes from https://app.squareup.com/digital-wallets/apple-pay/apple-developer-merchantid-domain-association
  (Square may update it; re-download and commit if Apple Pay registration ever needs to be redone).
* Do not add a custom domain (CNAME) here: it would also move every project site.
