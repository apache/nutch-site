+++
title = "Downloads"
description = "The primary resource for all official Nutch releases"
weight = 10
draft = false
toc = true
bref = ""
+++

# Download
Apache Nutch 1.19 (src-tar, src-zip, bin-tar and bin-zip) and 2.4 (src-tar and src-zip only) can be downloaded from the table below. See

* [CHANGES-1.19.txt](https://apache.org/dist/nutch/1.19/CHANGES.txt) (released 2022-08-22), and
* [CHANGES-2.4.txt](https://apache.org/dist/nutch/2.4/CHANGES.txt) (released 2019-10-11)

for more information on the list of updates in these releases.

All Apache Nutch distributions is distributed under the [Apache License, version 2.0](https://www.apache.org/licenses/LICENSE-2.0.html).

The link in the Mirrors column below should display a list of available mirrors with a default selection based on your inferred location. If you do not see that page, try a different browser. The checksum and signature are links to the originals on the main distribution server.

| **Version**                    | **Mirrors**                                                                                                   | **Checksum**                                                                                                  | **Signature**                                                                                           |
|--------------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| Apache Nutch 1.19 (src.tar.gz) | [apache-nutch-1.19-src.tar.gz](https://www.apache.org/dyn/closer.lua/nutch/1.19/apache-nutch-1.19-src.tar.gz) | [apache-nutch-1.19-src.tar.gz.sha512](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-src.tar.gz.sha512) | [apache-nutch-1.19-src.tar.gz.asc](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-src.tar.gz.asc) |
| Apache Nutch 1.19 (src.zip)    | [apache-nutch-1.19-src.zip](https://www.apache.org/dyn/closer.lua/nutch/1.19/apache-nutch-1.19-src.zip)       | [apache-nutch-1.19-src.zip.sha512](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-src.zip.sha512)       | [apache-nutch-1.19-src.zip.asc](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-src.zip.asc)       |
| Apache Nutch 1.19 (bin.tar.gz) | [apache-nutch-1.19-bin.tar.gz](https://www.apache.org/dyn/closer.lua/nutch/1.19/apache-nutch-1.19-bin.tar.gz) | [apache-nutch-1.19-bin.tar.gz.sha512](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-bin.tar.gz.sha512) | [apache-nutch-1.19-bin.tar.gz.asc](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-bin.tar.gz.asc) |
| Apache Nutch 1.19 (bin.zip)    | [apache-nutch-1.19-bin.zip](https://www.apache.org/dyn/closer.lua/nutch/1.19/apache-nutch-1.19-bin.zip)       | [apache-nutch-1.19-bin.zip.sha512](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-bin.zip.sha512)       | [apache-nutch-1.19-bin.zip.asc](https://apache.org/dist/nutch/1.19/apache-nutch-1.19-bin.zip.asc)       |
| Apache Nutch 2.4 (src.tar.gz)  | [apache-nutch-2.4-src.tar.gz](https://www.apache.org/dyn/closer.lua/nutch/2.4/apache-nutch-2.4-src.tar.gz)    | [apache-nutch-2.4-src.tar.gz.sha512](https://apache.org/dist/nutch/2.4/apache-nutch-2.4-src.tar.gz.sha512)    | [apache-nutch-2.4-src.tar.gz.asc](https://apache.org/dist/nutch/2.4/apache-nutch-2.4-src.tar.gz.asc)    |
| Apache Nutch 2.4 (src.zip)     | [apache-nutch-2.4-src.zip](https://www.apache.org/dyn/closer.lua/nutch/2.4/apache-nutch-2.4-src.zip)          | [apache-nutch-2.4-src.zip.sha512](https://apache.org/dist/nutch/2.4/apache-nutch-2.4-src.zip.sha512)          | [apache-nutch-2.4-src.zip.asc](https://apache.org/dist/nutch/2.4/apache-nutch-2.4-src.zip.asc)          |
|                                |                                                                                                               |                                                                                                               |                                                                                                         |

# Verify Releases
It is essential that you verify the integrity of the downloaded files using the PGP or SHA signatures (MD5 for older releases). Please read [Verifying Apache HTTP Server Releases](https://httpd.apache.org/dev/verification.html) for more information on why you should verify our releases. We strongly recommend you verify your downloads with ASC and SHA512 signatures.

## PGP Signature
The PGP signatures can be verified using `PGP` First download the [KEYS](https://www.apache.org/dist/nutch/KEYS) as well as the `asc` signature file for the relevant distribution. Make sure you get these files from the [main distribution directory](https://www.apache.org/dist/nutch/), rather than from a mirror. Then verify the signatures using

```
$ gpg --import KEYS
$ gpg --verify apache-nutch-X.Y.Z-src.tar.gz.asc apache-nutch-X.Y.Z-src.tar.gz
```
Make sure to change the file names to match package, version and format.

The files in Apache Nutch 1.19 releases are signed by Sebastian Nagel (snagel) `48BAEBF6`. The files in Apache Nutch 2.4 release are signed by Sebastian Nagel (snagel) `DB0A9C6D`.

## SHA Signature
Additionally, you can verify the SHA signature on the files. A Unix program called **shasum** or **sha512sum** is included in many Unix distributions.
```
$ sha512sum --check apache-nutch-X.Y.Z.sha512
```

## MD5 Signature
Older releases used the MD5 signature. You may use the Unix program **md5** or **md5sum** to verify the MD5 signature:
```
$ md5sum apache-nutch-X.Y.Z
```
... output should match the string in `apache-nutch-X.Y.Z.md5`.

# Previous Releases
If you are looking for previous releases of Apache Nutch, have a look in the [Apache Archives](https://archive.apache.org/dist/nutch/).

Subscribe to the `dev [at] apache [dot] org` [mailing list](/community/mailing-lists/) if you want to get notified about future release candidates and subsequent Nutch official releases.

Apache Nutch releases are available under the Apache License, Version 2.0. See the NOTICE.txt file contained in each release artifact for applicable copyright attribution notices.