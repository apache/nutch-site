Nutch Website
=============

<img src="https://nutch.apache.org/assets/img/nutch_logo_tm.png" align="right" width="300" />

This repository contains the website source code for the [Apache Nutch](https://nutch.apache.org) project.

# Credits
Built using the [kube Theme for Hugo](https://github.com/jeblister/kube). 

# Tooling

The Website is built using [Hugo](https://gohugo.io/) a popular open-source static website generation framework.

# Prerequisites
* [Install Hugo](https://gohugo.io/getting-started/installing/)

# Serve the Site Locally

Change into the project directory and execute

```bash
$ hugo server -w
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

# Creating new Content

Check out the [Kube documentation](https://github.com/jeblister/kube#getting-started). Any further questions should be asked on the [Nutch dev@ mailing list](https://nutch.apache.org/community/mailing-lists/).

# Contributing

The [process is the same](https://github.com/apache/nutch?tab=readme-ov-file#contributing) as for the Nutch codebase.

# Building and Publishing the Site

To deploy a static site build execute
```
hugo --destination static_site
```

The static site is kept in this directory in the branch `asf-site` in the folder `content/` and automatically deployed onto the public Nutch website. See the [Apache Infra project website docs](https://infra.apache.org/project-site.html) and the configuration file [.asf.yaml](./asf.yaml). The branch `asf-staging` is used for deploying the staging site https://nutch.staged.apache.org/.


# License
Licensed under the [Apache Licence v2](https://www.apache.org/licenses/LICENSE-2.0)
