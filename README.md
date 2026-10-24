# Personal tvOS browser build

Builds an unsigned IPA from the fixed source commit in [jvanakker/tvOSBrowser PR 68](https://github.com/jvanakker/tvOSBrowser/pull/68). The fork commit is pinned to 81ae5490d6a850a427e75f42f519aeadf69778f3.

The workflow uses GitHub's Xcode 27 preview runner, builds Debug (matching the upstream contributor's device test), and retains the unsigned artifact for three days. It runs only when the build workflow is pushed or started manually. There is no schedule.

No Apple account, signing certificate, device identifier, local IP address or subscription is required or included. Download the IPA and sign it locally before installation. This repository does not distribute the app through the App Store.

The upstream report covers one tvOS 27 beta device. Building successfully does not establish compatibility with every tvOS version; installation and browser behavior require device testing.
