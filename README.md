Nutch Website
=============

<img src="https://nutch.apache.org/assets/img/nutch_logo_tm.png" align="right" width="300" />

This repository contains the website source code for the [Apache Nutch](https://nutch.apache.org) project.

# Tooling

The Website is built using [Hugo](https://gohugo.io/) a popular open-source static website generation framework.

# Prerequisites
* [Install Hugo](https://gohugo.io/getting-started/installing/)

# Local Build and Deploy

```bash
$ hugo server
...
Start building sites …

                   | EN
-------------------+-----
  Pages            | 10
  Paginator pages  |  0
  Non-page files   |  0
  Static files     | 10
  Processed images |  0
  Aliases          |  0
  Sitemaps         |  1
  Cleaned          |  0

Built in 107 ms
Watching for changes in /path/to/nutch_site/{archetypes,content,data,layouts,static,themes}
Watching for config changes in /path/to/nutch_site/config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

# Contributing

To contribute a patch, follow these instructions (note that installing
[Hub](https://hub.github.com/) is not strictly required, but is recommended).

```
0. Download and install hub.github.com
1. File JIRA issue for your fix at https://issues.apache.org/jira/projects/NUTCH/issues
- you will get issue id NUTCH-xxx where xxx is the issue ID.
2. git clone https://github.com/apache/nutch-site.git
3. cd nutch-site
4. git checkout -b NUTCH-xxx
5. edit files
6. git status (make sure it shows what files you expected to edit)
7. git add <files>
8. git commit -m “fix for NUTCH-xxx contributed by <your username>”
9. git fork
10. git push -u <your git username> NUTCH-xxx
11. git pull-request
```

# License
