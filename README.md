# Baseline Abode Initiative

A conceptual BAU calculator and manifesto. The proposed rule allocates **1,000 EC per participating individual per year**, independent of local currency. No live EC issuance or redemption is implemented.

The comparison panel converts the same annual EC allocation using editable USD reference, market INR/USD rate, material costs per square foot, and material allocation percentage. Its housing-material purchasing-power rate is `India INR/ft² ÷ U.S. USD/ft²`; its area ratio is `market INR/USD ÷ housing-material rate`. Defaults are illustrative assumptions, not live market data or identical construction specifications. The main BAU projection uses separate hypothetical annualization and allocation assumptions; its guaranteed floor is not independently funded by the model.

## Offline use

The web manifest and service worker precache both pages, both stylesheets, the manifest and icons. Visit once online and allow the service worker to install before disconnecting. On iOS Safari, use Share → Add to Home Screen; offline behavior depends on WebKit retaining site data. The calculator does not need a network API.

Run locally over HTTP (not `file://`):

```bash
python -m http.server 8080
```

Then visit `http://localhost:8080/`. For an offline test, load both pages, wait for `navigator.serviceWorker.ready`, disconnect the browser network, and reload the installed page and manifesto.
