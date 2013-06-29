---
layout: post
title: Managing Print Files with Box net
url: http://kinlane.com/2011/04/30/3509/
image: http://kinlane-productions.s3.amazonaws.com/cloud-storage/Box-logo-new.jpg
---
{% include JB/setup %}

One such platform that I've identified as a Mimeo.com partner platform is <a title="Box.net" href="http://www.box.net">Box.net</a>.
Box.net provides a complete cloud storage platform, with a powerful developer platform and application directory called OpenBox.
Mimeo.com provides commercial web to print services, and with Mimeo Connect Cloud Print API you can integrate print file management from Box.net
<em>*** Heads up!! This requires basic understanding of box.net and programming with PHP ***</em>
To do this I sign up for a <a title="Box.net Developer Account" href="http://www.box.net/developers">Box.net developers account</a> and add new OpenBox application:
<ul class="blue">
     <li>Give Application Name and Description
     </li>
     <li>Assign a description page for the application that tells about my printer.
     </li>
</ul>An important part of this application is a callback URL for when users first add the Box.net application. This has to be a page you host that handles the Box.net oAuth, which gives this print file manager access to a users account.
Another important part of each application are whats called <em>service actions</em>. Service actions which will show up for any user who adds this application to their Box.net account from OpenBox.
For my Open Box Application I create a new service action: <img src="http://kinlane-productions.s3.amazonaws.com/Box.net/Open-Box.png"  width="250" align="right" />
<ul class="blue">
     <li>Give Application Service Action a title like, <strong><em>Send Print File toMimeo</em></strong>
     </li>
     <li>Choose which document extensions my print file manager supports, PDF for now
     </li>
     <li>Enter a callback function which Box.net will send user when printing document
     </li>
     <li>Enter callback parameters such as URL, Title, Extension of Box.net file to be printed.
     </li>
</ul>Save your service action, fill out any other relevant parts of your application and hit save as well.
This creates your application at Box.net.
Now you need put together the code that integrates Box.net with your Mimeo.com account using the Mimeo Connect Cloud Print API.
First you need the OAuth piece of code described above, you can <a title="download at Github" href="https://github.com/mimeoconnect/Mimeo-Box.net">download this at Github</a>. It requires the following files:
<ul class="blue">
     <li>box_config.php
     </li>
     <li>boxlibphp5.php
     </li>
     <li>class.curl.php
     </li>
     <li>index.php
     </li>
</ul>This will allow your print file manager to OAuth with Box.net.
Now you need the actual code that lets you pull the file being passed by Box.net and print uses Mimeo.com.
Here is a sample code file for doing this:

The above code sample demonstrates how to build a <a title="print file manager using Box.net cloud storage and Mimeo Connect Cloud Print API" href="http://developer.mimeo.com/blog/blog_detail.php?ID=92">print file manager using Box.net cloud storage and Mimeo Connect Cloud Print API</a>.
Any company can use Box.net to manage their print files, and allow commercial printing using Mimeo.com
You can dowload a complete library of <a title="PHP code samples for integrating Box.net with Mimeo.com" href="https://github.com/mimeoconnect/Mimeo-Box.net">PHP code samples for integrating Box.net with Mimeo.com</a> at Github.