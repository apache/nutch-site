+++
title = "Downloads"
description = "The primary resource for all official Nutch releases"
weight = 10
draft = false
toc = true
bref = ""
+++

# Download
Apache Nutch {{< param nutchVersion >}} (src-tar, src-zip, bin-tar and bin-zip) artifacts can be downloaded from the table below. See [CHANGES.md](https://apache.org/dist/nutch/{{< param nutchVersion >}}/CHANGES.md) for the comprehensive change log for Nutch {{< param nutchVersion >}} released on 2024-04-24 (YYYY-MM-DD).

All Apache Nutch distributions is distributed under the [Apache License, version 2.0](https://www.apache.org/licenses/LICENSE-2.0.html). See the NOTICE.txt file contained in each Nutch release artifact for applicable copyright attribution notices.

The link in the Mirrors column below should display a list of available mirrors with a default selection based on your inferred location. If you do not see that page, try a different browser. The sha512 checksum and ASC signature are links to the originals on the main distribution server.

| **Version**                    | **Mirrors**                                                                                                   | **Checksum**                                                                                                  | **Signature**                                                                                           |
|--------------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| Apache Nutch {{< param nutchVersion >}} (src.tar.gz) | [apache-nutch-{{< param nutchVersion >}}-src.tar.gz](https://www.apache.org/dyn/closer.lua/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-src.tar.gz) | [apache-nutch-{{< param nutchVersion >}}-src.tar.gz.sha512](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-src.tar.gz.sha512) | [apache-nutch-{{< param nutchVersion >}}-src.tar.gz.asc](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-src.tar.gz.asc) |
| Apache Nutch {{< param nutchVersion >}} (src.zip)    | [apache-nutch-{{< param nutchVersion >}}-src.zip](https://www.apache.org/dyn/closer.lua/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-src.zip)       | [apache-nutch-{{< param nutchVersion >}}-src.zip.sha512](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-src.zip.sha512)       | [apache-nutch-{{< param nutchVersion >}}-src.zip.asc](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-src.zip.asc)       |
| Apache Nutch {{< param nutchVersion >}} (bin.tar.gz) | [apache-nutch-{{< param nutchVersion >}}-bin.tar.gz](https://www.apache.org/dyn/closer.lua/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-bin.tar.gz) | [apache-nutch-{{< param nutchVersion >}}-bin.tar.gz.sha512](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-bin.tar.gz.sha512) | [apache-nutch-{{< param nutchVersion >}}-bin.tar.gz.asc](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-bin.tar.gz.asc) |
| Apache Nutch {{< param nutchVersion >}} (bin.zip)    | [apache-nutch-{{< param nutchVersion >}}-bin.zip](https://www.apache.org/dyn/closer.lua/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-bin.zip)       | [apache-nutch-{{< param nutchVersion >}}-bin.zip.sha512](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-bin.zip.sha512)       | [apache-nutch-{{< param nutchVersion >}}-bin.zip.asc](https://apache.org/dist/nutch/{{< param nutchVersion >}}/apache-nutch-{{< param nutchVersion >}}-bin.zip.asc)       |

# Verify Releases
It is essential that you verify the integrity of the downloaded files using the PGP or SHA signatures (MD5 for older releases). Please read [Verifying Apache HTTP Server Releases](https://httpd.apache.org/dev/verification.html) for more information on why you should verify our releases. We strongly recommend you verify your downloads with ASC and SHA512 signatures.

## PGP Signature
The PGP signatures can be verified using `PGP` First download the [KEYS](https://www.apache.org/dist/nutch/KEYS) as well as the `asc` signature file for the relevant distribution. Make sure you get these files from the [main distribution directory](https://www.apache.org/dist/nutch/), rather than from a mirror. Then verify the signatures using

```
$ gpg --import KEYS
$ gpg --verify apache-nutch-{{< param nutchVersion >}}-src.tar.gz.asc apache-nutch-{{< param nutchVersion >}}-src.tar.gz
```
Make sure to change the file names to match package, version and format.

The files in Apache Nutch {{< param nutchVersion >}} releases are signed by Lewis John McGibbney (lewismc) `48BAEBF6`.

## SHA Signature
Additionally, you can verify the SHA signature on the files. A Unix program called **shasum** or **sha512sum** is included in many Unix distributions.
```
$ sha512sum --check apache-nutch-{{< param nutchVersion >}}-src.tar.gz.sha512
```

# Previous Releases
If you are looking for previous releases of Apache Nutch, have a look in the [Apache Archives](https://archive.apache.org/dist/nutch/).

Subscribe to the `dev [at] apache [dot] org` [mailing list](/community/mailing-lists/) if you want to get notified about future release candidates and subsequent Nutch official releases.
