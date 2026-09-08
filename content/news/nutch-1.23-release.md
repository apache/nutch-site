+++
date = "2026-09-08"
title = "Nutch 1.23 Release"
tags = ["1.23","release"]
categories = ["releases"]
draft = false
description = "8 September 2026 – Apache Nutch 1.23 released"
weight = 10
+++

The <a href="https://projects.apache.org/committee.html?nutch" target="_blank">Apache Nutch PMC</a> are pleased to announce the immediate release of **Apache Nutch v1.23**, we advise all current users and developers of the 1.X series to upgrade to this release.

<div id="action-buttons">
  <a class="button primary big" href="/download" onclick="_gaq.push(['_trackEvent', 'kube', 'download']);">Download Nutch 1.23</a>
</div>

You may also be interested in the <a href="https://s.apache.org/c4qjb" target="_blank">1.23 release report</a> and the breaking changes:
- Nutch requires JDK 17 at build and runtime.
- The minimum required Hadoop version is 3.5.0 if Nutch is run on a Hadoop cluster.
- [NUTCH-1732](https://issues.apache.org/jira/browse/NUTCH-1732) introduced a new CrawlDatum status,
  `db_parse_failed`. A CrawlDb written with Nutch 1.23 might fail to be read with older Nutch versions,
  if it contains records with status `db_parse_failed`. As the name indicates, the status marks
  documents which failed to parse. It is only set if the property `parser.delete.failed.parse` is
  `true` (default: `false`). If your workflow requires that Nutch data can be read with Nutch 1.22
  (or older), please keep the property set to `false`.

In the 1.X series, release artifacts are made available as both source and binary and also available within <a href="https://search.maven.org/search?q=g:org.apache.nutch%20AND%20a:nutch%20AND%20v:1.23" target="_blank">Maven Central</a>.
