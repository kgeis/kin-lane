---
layout: post
title: Google Cloud Print Proxy Cloud Printer
url: http://kinlane.com/2011/02/08/google-cloud-print-proxy-cloud-printer/
image: http://kinlane-productions.s3.amazonaws.com/mimeo-logo.jpg
---
{% include JB/setup %}

I have written specific blog posts for each service endpoint, and to finish up I wanted to do a complete walk-through.
First I authenticate against a users Google Account with <a href="http://code.google.com/apis/accounts/docs/AuthForInstalledApps.html" target="_blank">Google ClientLogin API</a>.
Then using the <a href="http://code.google.com/apis/cloudprint/docs/proxyinterfaces.html" target="_blank">Google Cloud Print Services Interface</a>:
<ul>
     <li>
          <a href="http://www.google.com/cloudprint/interface/" target="_blank">http://www.google.com/cloudprint/interface/</a>
     </li>
</ul>I can make calls to the following end points to manage printers:
<ul>
     <li>
          <a href="http://www.kinlane.com/2011/02/google-cloud-print-register/" target="_blank">/register</a>
     </li>
     <li>
          <a href="http://www.kinlane.com/2011/02/google-cloud-print-list/" target="_blank">/list</a>
     </li>
     <li>
          <a href="http://www.kinlane.com/2011/02/google-cloud-print-update/" target="_blank">/update</a>
     </li>
     <li>
          <a href="http://www.kinlane.com/2011/02/google-cloud-print-delete/" target="_blank">/delete</a>
     </li>
</ul>I can make calls to the following end points to manage cloud print jobs:
<ul>
     <li>
          <a href="http://www.kinlane.com/2011/02/2822/" target="_blank">/fetch</a>
     </li>
     <li>
          <a href="http://www.kinlane.com/2011/02/google-cloud-print-control/" target="_blank">/control</a>
     </li>
</ul>You can receive print job notifications via persistent XMPP connection:
<ul>
     <li>
          <a title="XMPP Print Job Notifications" href="http://www.kinlane.com/2011/02/google-cloud-print-xmpp-print-job-notifications/">XMPP Print Job Notifications</a>
     </li>
</ul>If you want to download the sample code for my Google Cloud Print Proxy work, you can download in the following formats:
<ul>
     <li>
          <a href="https://github.com/mimeoconnect/Google-Cloud-Print-Proxyreadme" target="_blank">git - Github</a>
     </li>
     <li>
          <a href="http://code.google.com/p/google-cloud-print-proxy/" target="_blank">svn - Google Code</a>
     </li>
</ul>If you have any thoughts or ideas for an innovative Cloud Print Proxy, let me know.
<a href="http://www.mimeo.com/"><img src="http://kinlane-productions.s3.amazonaws.com/google-cloud-print/google-cloud-print-mimeo.png"  width="500" align="center" /></a>
 
<strong>UPDATE 2/28/2011 -</strong> I have finished the first prototype for the <a title="XMPP Print Job Notification Service" href="http://www.kinlane.com/2011/02/google-cloud-print-xmpp-print-job-notifications/">XMPP print job notification service</a>. This is critical piece to eliminate constant polling of /fetch service.
<h6 class="zemanta-related-title c3">
     Related articles
</h6>
<ul class="zemanta-article-ul">
     <li class="zemanta-article-ul-li">
          <a href="http://www.readwriteweb.com/archives/cloud_print_coming_soon_to_google_docs.php">Cloud Print "Coming Soon" to Google Docs</a> (readwriteweb.com)
     </li>
     <li class="zemanta-article-ul-li">
          <a href="http://go.theregister.com/feed/www.theregister.co.uk/2010/12/08/google_cloud_print/">Google sees printing in the cloud</a> (go.theregister.com)
     </li>
     <li class="zemanta-article-ul-li">
          <a href="http://downloadsquad.switched.com/2010/12/07/google-cloud-print-is-now-available/">Google Cloud Print is now available</a> (downloadsquad.switched.com)
     </li>
</ul>