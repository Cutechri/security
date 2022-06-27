# Introduction
This file details all the Microsoft Edge flags that have been modified in my [security guide](https://cutechri.com/#security).

## Enabled flags

| Name | Description |
| :--- | :---------- |
| #isolate-origins | Contributes to the Chromium site isolation model |
| #disallow-doc-written-script-loads | Helps against fingerprinting related exploits |
| #block-insecure-private-network-requests | Self-explanatory |
| #edge-automatic-https | Enforces HTTPS on all sites |
| #edge-autoplay-user-setting-block-option | Blocks autoplay of potentially harmful media |
| #edge-enable-bfcache-features | Enables the back-forward cache  |
| #edge-wdag-optional-network-isolation | Strengthens MDAG network isolation |
| #edge-experimental-tracking-prevention-features | Enables additional tracking prevention improvements |
| #edge-robin | Enables [Project Robin](https://techcommunity.microsoft.com/t5/discussions/introducing-project-robin-new-feature/m-p/2264484) - broken, keep it on in case it works again |
| #strict-origin-isolation | Further strengthens Chromium's site isolation |
| #partitioned-cookies | Isolates and partitions the cookies for improved security |

## Disabled flags
| Name | Description |
| :--- | :---------- |
| #enable-webrtc-remote-event-log | Block WebRTC remote logs |
| #show-autofill-type-predictions | Blocks placeholder text in autofill boxes |
| #media-router-cast-allow-all-ips | Does not allow all IPs to cast |
| #enable-generic-sensor-extra-classes | Disables bleeding edge sensor related code |
| #edge-log-textfield-lag | Disables logging of omnibox lag |
| #edge-playready-drm-win10 | Disables PlayReady DRM - **needed for Spotify, Netflix, etc.** |
| #edge-widevine-drm | Disables WideVine DRM - **needed for Spotify, Netflix, etc.** |
| #edge-haptics-api | Disables additional unneeded haptics code |
| #edge-toast-winrt | Disables background tasks managing toast notifications |
| #file-handling-api | Disables the ability of malicious sites registering as persistent file handlers |
| #web-bundles | Disables experimental web bundle code, unnecessary |
| #trust-tokens | Disables the prototype trust token API, security risk |
| #enable-prerender2 | Disables the new prerenderer implementation sticking with the tried and trusted one |
| #enable-first-party-sets | Disables potentially malicious first party cookies |
| #sameparty-cookies-considered-first-party | Ditto |
