# Iglu Central

[![Build Status][cd-image]][cd] [![Release][release-image]][releases] [![License][license-image]][license]

Iglu Central (**[website][iglucentral-website]**) is a central repository for storing JSON Schemas, Avros and Thrifts, maintained and hosted by the team at **[Snowplow Analytics][snowplow-website]**. Think of it like RubyGems.org or Maven Central but for storing data schemas instead of code.

All of the schemas for **[Snowplow][snowplow-repo]** (amongst other systems) are stored in Iglu Central.

![iglucentral-img][iglucentral-img]

## Dev registries

Iglu Central automatically publishes content of pull requests opened by users with write permissions to a static S3 registry.
Full path of a dev registry is:

```
http://iglucentral-dev.com.s3-website-us-east-1.amazonaws.com/BRANCH_NAME
```

Where `BRANCH_NAME` is the name of git branch in the PR. This registry can be used in a resolver configuration until PR is merged into master branch.

Another option for temporary registry is to use Github raw hosting:

```
https://raw.githubusercontent.com/snowplow/iglu-central/BRANCH_NAME
```

Where `snowplow` can be replaced with your Github username if you forked the repository.

## Find out more

| **[Technical Docs][techdocs]**     | **[Setup Guide][setup]**     | **[Roadmap][roadmap]**           | **[Contributing][contributing]**           |
|-------------------------------------|-------------------------------|-----------------------------------|---------------------------------------------|
| [![i1][techdocs-image]][techdocs] | [![i2][setup-image]][setup] | [![i3][roadmap-image]][roadmap] | [![i4][contributing-image]][contributing] |

## Copyright and license

Iglu Central is copyright 2014-2021 Snowplow Analytics Ltd.

Licensed under the **[Apache License, Version 2.0][license]** (the "License");
you may not use this software except in compliance with the License.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

[cd]: https://github.com/snowplow/iglu-central/actions?query=workflow%3ACI
[cd-image]: https://github.com/snowplow/iglu-central/workflows/CI/badge.svg

[release-image]: http://img.shields.io/badge/release-121-orange.svg?style=flat
[releases]: https://github.com/snowplow/iglu-central/releases

[license-image]: http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat
[license]: http://www.apache.org/licenses/LICENSE-2.0

[iglucentral-website]: http://iglucentral.com
[snowplow-repo]: https://github.com/snowplow/snowplow
[snowplow-wiki]: https://github.com/snowplow/snowplow/wiki
[snowplow-website]: http://snowplowanalytics.com

[iglucentral-img]: https://github.com/snowplow/iglu/wiki/technical-documentation/images/iglu-central.png

[techdocs-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
[setup-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
[roadmap-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/roadmap.png
[contributing-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png

[techdocs]: https://github.com/snowplow/iglu/wiki/Iglu-Central
[setup]: https://github.com/snowplow/iglu/wiki/Iglu-Central-setup
[roadmap]: https://github.com/snowplow/iglu/wiki/Product-roadmap
[contributing]: https://github.com/snowplow/iglu/wiki/Contributing-to-Iglu-Central
