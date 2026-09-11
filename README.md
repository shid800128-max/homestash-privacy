# HomeStash — privacy policy

The public privacy policy for the HomeStash Android app
(`com.boen.homestash`), served by GitHub Pages so the Play Console has a
URL to point at.

**Live URL:** https://shid800128-max.github.io/homestash-privacy/

This repository is public on purpose — the policy has to be reachable without
signing in, or Play rejects the listing. It contains nothing but this page.
The app's source lives in a separate, private repository.

## Publishing it

1. Create a **public** repo named `homestash-privacy` under `shid800128-max`.
2. Push this directory to it.
3. Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)`.
4. Wait a minute, then open the URL above and check it loads **while signed
   out** (a private window). Play's reviewer is not logged into your account.

## Keeping it honest

The policy claims the app cannot reach the network. That is currently true and
verifiable: the release package declares no `INTERNET` permission.

```bash
aapt2 dump permissions app-release.apk
```

**That claim stops being true the moment cloud sync lands (M3).** Adding the
internet permission, an account, or the photo-recognition call means this page
and the Play Data safety form both have to be updated in the same release —
not after it. A stale privacy policy is a compliance problem, not a
documentation one.
