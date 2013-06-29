---
layout: post
title: Proofing Print Documents From Amazon S3
url: http://kinlane.com/2011/01/26/proofing-print-documents-from-amazon-s3/
image: http://kinlane-productions.s3.amazonaws.com/AWS_LOGO_CMYK.jpg
---
{% include JB/setup %}

You will need:
<ul>
     <li>
          <a href="http://aws.amazon.com/" target="_blank">Amazon Web Services Account</a>
     </li>
     <li>
          <a href="http://www.mimeo.com/" target="_blank">Mimeo API Account.</a>
     </li>
</ul>This <a href="http://www.kinlane.com/category/cloud-computing/cloud-print/">Cloud Print</a> demonstration is written in <a href="http://www.kinlane.com/category/php/">PHP</a>, and uses the <a href="https://github.com/mimeoconnect/Mimeo-Connect-Cloud-Print-API---REST-Client" target="_blank">Mimeo Connect Cloud Print API REST Client</a>. <a href="http://www.mimeo.com" target="_blank"><img src="http://kinlane-productions.s3.amazonaws.com/mimeo-logo.jpg"  width="250" align="right" /></a> You can download the source code for the <a href="http://www.kinlane.com/category/amazon/amazon-s3/">Amazon S3</a> to Mimeo Connect project in the following formats:
<ul>
     <li>
          <a href="https://github.com/mimeoconnect/mimeo-amazon-s3" target="_blank">git (GitHub Repository) - Amazon S3 to Mimeo Print</a>
     </li>
     <li>
          <a href="https://code.google.com/p/amazon-s3-mimeo/" target="_blank">svn (Google Code Project - Amazon S3 to Mimeo Print</a>
     </li>
</ul>I will be updating this project when I develop any new code that integrates Amazon S3 and the Mimeo Connect Cloud Print API.
This project currently allows you to pull print files from Amazon S3 and proof them with Mimeo Connect Cloud Print API and preview or view any pages in the PDF as images in Flash or <a href="http://www.kinlane.com/2011/01/jquery-powered-flipbook-for-previewing-print-files/">JQuery Flipbook</a>.