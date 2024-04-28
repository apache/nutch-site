+++
title = "SysAdmins/WebMasters"
description = "A page for SysAdmins/WebMasters and other angry people... ;)"
weight = 10
draft = false
toc = true
bref = ""
+++

# Introduction
If you're reading this, chances are you've seen a Nutch-based robot visiting your site while looking through your server logs. Our software obeys robots.txt files and robot META tags in HTML. These are the standard mechanisms for webmasters to tell web robots which portions of a site a robot is welcome to access.

# Sysadmins/robots.txt
We're a software project, not a service, so please understand that a misbehaving crawler appearing with our Agent string is not run by us. Our software may be run by anyone. However, we'd still like to hear about any bad behavior. If possible, please include the name of the domain and some representative log entries. We can be reached at `dev[at]nutch[dot]apache[dot]org`

Our software obeys the <a href="http://www.robotstxt.org/robotstxt.html" target="_blank">robots.txt exclusion standard</a>. Different Nutch deployments may specify different agent names, but all should respond to the agent name "Nutch". Thus to ban all Nutch-based crawlers from your site, place the following in your robots.txt file:

```
User-agent: Nutch
Disallow: /
```

# Webmasters/Robots META
 If you do not have permission to edit the `/robots.txt` file on your server, you can still tell robots not to index your pages or follow your links. The standard mechanism for this is the <a href="http://www.robotstxt.org/meta.html" target="_blank">robots META tag</a>.