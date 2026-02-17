+++
date = "2014-09-22T00:00:00+00:00"
title = "Wicket WebApp now part of Nutch 2.x Codebase"
tags = ["webapp","wicket","GSoC"]
categories = ["news"]
draft = false
description = "22 September 2014 - Wicket WebApp now part of Nutch 2.x Codebase"
weight = 10
+++

After successful completion of the first [Nutch Google Summer of Code project](https://issues.apache.org/jira/browse/NUTCH-841)
we are pleased to announce that Nutch 2.X branch now comes packaged with a self 
contained [Apache Wicket](https://wicket.apache.org/)-based Web Application.

This not only greatly lowers the barrier for direct interaction with the Nutch 2.X
REST API but also provides a stepping stone from which we intend to backport this 
work to the Nutch 1.X (trunk) series.

Some of the Web Application features include:

  * Functionality to dynamically load seed URLs in order to bootstrap Nutch crawls
  * Browsable and dynamic editing of [Configuration overrides](https://cwiki.apache.org/nutch/NutchPropertiesCompleteList)
  * Complete [REST API documentation](https://cwiki.apache.org/nutch/NutchRESTAPI) and UML
model describing REST API calls, Administration and Job and Configuration Management.

The new Web Application feature will be present within the upcoming Nutch 2.3 Release.
