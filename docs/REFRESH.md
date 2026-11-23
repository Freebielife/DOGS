# DOGS refresh

The project uses `.github/workflows/update.yml`: source pushes, manual dispatch, and fallback schedule `7,37 * * * *` (UTC). Collection retains last good sections and records incomplete sources. GitHub schedules can be delayed.

The existing shared Cloudflare runner is `freebie-observatory-runner`. Do not deploy the template example registry. Add the following record to the full current shared registry only when authenticated deployment is available, preserving every existing project:

```js
Object.freeze({id:"dogs",owner:"Freebielife",repo:"DOGS",workflow:"update.yml",ref:"main",everyMinutes:30,phaseMinutes:10,enabled:true})
```

Grant the existing dispatcher token access to DOGS, deploy the preserved complete runner, observe a successful DOGS workflow_dispatch run, then remove the fallback schedule to avoid duplicate runs. No Cloudflare deployment was performed during initial preparation because the dashboard required authentication.
