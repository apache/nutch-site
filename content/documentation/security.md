+++
title = "Security"
description = "Reporting Nutch security issues and an explanation of the Nutch security model"
weight = 10
draft = false
toc = true
bref = ""

+++

## Reporting Security Issues of Apache Nutch

The Apache Software Foundation is very active in eliminating security problems and denial-of-service attacks against its products.

We strongly encourage people to report security issues privately via the [ASF Security Team](https://www.apache.org/security/)'s mailing list before disclosing them publicly.

Please note that the security mailing list is intended solely for reporting undisclosed security vulnerabilities and managing the process of fixing them. We cannot accept regular bug reports or other queries at this address. Any email sent to this address that does not relate to an undisclosed security vulnerability in the Nutch source code will be ignored.

The private security mailing address is: security@apache.org

## Security Model

Apache Nutch is designed to operate in trusted environments, either locally or on a Hadoop cluster.

This section outlines the security model and key security considerations. Understanding how to use and deploy Nutch in a secure manner is mandatory.

#### Trusted Configuration

The configuration files used by Nutch are loaded during job execution. These files are treated as a trusted source and must not involve any user-supplied input at runtime.

#### Nutch Runtime

Nutch can be run on a local instance or on a Hadoop cluster. For both runtimes, it is mandatory that access to the runtime must be restricted to trusted users. Securing the Nutch runtime is essential. For information on securing a Hadoop cluster, please refer to the [Apache Hadoop security page](https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-common/SecureMode.html).

#### Nutch Server and REST API

Nutch releases which packaged the legacy JAX-RS Nutch service/server/REST API did not provide any authentication and/or authorization. Therefore the service must not be publicly available. Access should only be granted to trusted users. Granting access to the service is equivalent to granting access to the instance where the service is running. This includes permissions to write to the local filesystem and run any Java class available on the service's class path.

The legacy JAX-RS Nutch service was removed in Nutch 1.23.

#### Information Leakage

By default, Nutch is configured to "crawl" the local file system and intranet resources. Feeding an intranet search is a common use case for Nutch. Additionally, Nutch can crawl web sites that require authorization. If the crawled data is exposed to the public, whether as a search index or in any other data formats (e.g., WARC files), it is mandatory to ensure that no private resources are included in the given crawl.

Measures to prevent information leakage include:

* Disabling access to the local file system (disable the "protocol-file" plugin).
* Maintaining restrictive URL filters.
* Enabling IP address filters to prevent access to private IP address ranges.

An attacker may place arbitrary links on pages visited by the crawler, for example a link to `file:///etc/passwd`. The crawler configuration must ensure that such links are not followed.

## Security-Related Questions

If you have security-related questions, please contact the Nutch team over the [dev](mailto:dev@nutch.apache.org) or [user](mailto:user@nutch.apache.org) mailing list. See [Mailing Lists](/community/mailing-lists/) for more information.

## Known Security Vulnerabilities

The following security vulnerabilities are known:
- See the section about the [Nutch Server and REST API](#nutch-server-and-rest-api).

## Nutch CVE List

tbd.
