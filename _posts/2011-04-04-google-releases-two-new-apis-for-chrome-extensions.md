---
layout: post
title: Google Releases Two New APIs for Chrome Extensions
url: http://kinlane.com/2011/04/04/google-releases-two-new-apis-for-chrome-extensions/
image: http://kinlane-productions.s3.amazonaws.com/google-chrome-logo.jpg
---
{% include JB/setup %}

<ul>
     <li>
          <a title="Web Navigation Extension API" href="http://code.google.com/chrome/extensions/trunk/experimental.webNavigation.html">Web Navigation Extension API</a> - Allows extension developers to observe browser navigation events. The API therefore allows an extension to keep track of exactly what page the tab is showing, and how the user got there.
     </li>
     <li>
          <a title="Proxy Extension API" href="http://code.google.com/chrome/extensions/trunk/experimental.proxy.html">Proxy Extension API</a> - Allows users to configure Chrome's proxy settings via extensions. Proxies can be configured for the entire browser or independently for regular and incognito windows.
     </li>
</ul>You can test drive these new APIs by enabling Experimental Extension APIs.
Until the APIs are stable, they require explicit permission from users.