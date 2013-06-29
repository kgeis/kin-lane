---
layout: post
title: LinkedIn Open Sources IndexTank Search Technology
url: http://kinlane.com/2011/12/21/linkedin-open-sources-indextank-search-technology/
image: http://kinlane-productions.s3.amazonaws.com/linkedin/LinkedIn-Developer-Network.png
---
{% include JB/setup %}

The IndexTank technology has three separate toolsets:
<ul>
     <li>
          <strong>IndexEngine</strong> - A real-time fulltext search-and-indexing system designed to separate relevance signals from document text
     </li>
     <li>
          <strong>API</strong> - A RESTful interface that handles authentication, validation, and communication with the IndexEngine(s)
     </li>
     <li>
          <strong>Nebulizer</strong> - Multitenant framework to host and manage an unlimited number of indexes running over a layer of Infrastructure-as-a-Service
     </li>
</ul><a href="http://indextank.com/" target="_blank"><img src="http://kinlane-productions.s3.amazonaws.com/api-evangelist/indextank/indextank_logo.png"  width="250" align="right" /></a> An example of IndexTank in action is, Reddit, which runs on IndexEngine and the API.
They have the <a href="https://github.com/linkedin/indextank-engine">IndexTank Engine</a> and <a href="https://github.com/linkedin/indextank-service">IndexTank Service</a> code published at Github, and created a <a title="LinkedIn Group to Support It" href="http://www.linkedin.com/groups?gid=4224441">LinkedIn Group to support it</a>.