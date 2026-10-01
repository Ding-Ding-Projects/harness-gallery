# Handoff

## Current state

The dedicated public evidence repository is `Ding-Ding-Projects/harness-gallery`. The publication commit is `06ef4ba7237ed3dd3622cb916af8c852010c549e`. It is scoped to three reviewed Harness captures and their provenance. The source application is separate at `Ding-Ding-Projects/harness`.

The images use local fixture data. Their capture source commit is `c028c39eb07c55d84dcac937d438a05073d42c46`, their packaged executable SHA-256 is `efd01ac3a348b9fb17f992a1627a0f3ec9646b60d100b73fbabf8693901d0b39`, and their validated capture times are recorded in `evidence/inventory.json`. The packaged runtime is the one captured; later documentation commits did not change it.

## Publication verification

The GitHub Pages site is live at https://ding-ding-projects.github.io/harness-gallery/. GitHub Pages build `1251348905` for commit `06ef4ba7237ed3dd3622cb916af8c852010c549e` reached `built`. Anonymous HTTP GETs returned 200 for the page, JSON inventory, and all three PNGs. PNG content types were `image/png`, delivered byte counts matched 69,009, 71,819, and 80,039, and all three delivered SHA-256 values matched the inventory.

The canonical public-content scan passed for 10 text files and the publication commit message. No tests or new captures were run. The viewport layout has not been verified in a built browser.

The fresh gallery checkout had no configured `core.hooksPath` or pre-push dictionary-lock hook. The canonical public-content scan was run manually before each push. Installing or changing global hook infrastructure was outside this lane and remains an inherited setup gap.

## Remaining work

The static page documents its known limitations. It does not provide the broader shared page contract, and no full-conformance claim is made. Status Hub write authorization was not configured. The Material Designer creation/export flow was not exposed. No new captures were made.
