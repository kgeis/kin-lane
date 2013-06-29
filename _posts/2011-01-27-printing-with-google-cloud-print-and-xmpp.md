---
layout: post
title: Printing with Google Cloud Print and XMPP
url: http://kinlane.com/2011/01/27/printing-with-google-cloud-print-and-xmpp/
image: http://kinlane-productions.s3.amazonaws.com/xmpp_logo.png
---
{% include JB/setup %}

Once I register a commercial cloud print on the network, then authenticate with a user using <a href="http://code.google.com/apis/accounts/docs/OAuth.html" target="_blank">Google authentication and authorization APIs</a> the printer is ready for printing. Print jobs availability is then handled through <a href="http://www.google.com/talk/" target="_blank">Google Talk</a>, using a persistent XMPP connection.
I'm refreshing my memory on the <a href="http://xmpp.org/" target="_blank">XMPP standard</a> as well as researching four PHP XMPP classes:
<ul>
     <li>
          <a href="http://groups.google.com/group/loudmouth-dev?pli=1" target="_blank">Loudmouth</a>
     </li>
     <li>
          <a href="http://code.google.com/p/jaxl/" target="_blank">jaxl</a>
     </li>
     <li>
          <a href="http://code.google.com/p/xmpphp/" target="_blank">xmpphp</a>
     </li>
     <li>
          <a href="http://bricabrac.origo.ethz.ch/wiki/Eiffel_XMPP" target="_blank">Eiffel XMPP</a>
     </li>
</ul>Although XMPP has its roots in communication its fascinatng to see the innovation around it into other areas of real-time programming such as <a href="http://www.kinlane.com/category/cloud-computing/cloud-print/" target="_blank">cloud printing</a>.
Even though the core technology is stable, the XMPP community continues to define various XMPP extensions, ther is also an active community of open-source and commercial developers further pushing the boundaries of whats possible with XMPP.