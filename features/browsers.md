# Browsers

AnuBitux comes with two available browsers, Firefox and Tor browser.

The **Firefox browser** has been heavily customized to safeguard user's privacy and security. First of all, it includes a lot of useful and trusted addons, listed [here](browsers.md). It's settings have also been customized so that it does not store history and cookies and it is enough to close and launch it again to have a totally fresh browser, not easily linkable to the previous activity (the best way to obtain a fresh and clean environment is to reboot AnuBitux live). There are also other useful custom settings, i.e. the browser asks each time where to store downloads, in order to avoid that some files may be automatically downloaded but the biggest work has been done in the about:config menu. To see the changes it is enough to type

```
about:config
```

in the URL bar and flag the "Show only modified preferences" option. There have been several changes to avoid telemetry, sponsored links, the use of any cache memory, the use of dangerous protocols like WebRTC, the execution of undesired scripts stored in .pdf files, and even a lot more!

<figure><img src="../.gitbook/assets/2024-04-06_17-00.png" alt=""><figcaption></figcaption></figure>

**Tor browser**, instead, has been included as is, since the Tor Project is taking a lot of effort in providing a very fine tuned browser, optimized to surf the Tor Network.
