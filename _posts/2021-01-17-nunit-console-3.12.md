---
layout: post
title:  "NUnit Console and Engine 3.12 Released"
date:   2021-01-17 12:00:00 -0000
categories: news update nunit
---

This release contains various improvements to running tests on .NET Core and Mono, and changes to
extension loading logic to allow the Engine to better support extensions which target multiple platforms. There are additionally
a number of fixes to issues that were identified with 3.12 Beta 1. Please also be aware that this will be the last version of
the NUnit Engine to support .NET Standard 1.6.

The .NET Core Console remains in Beta due to some unresolved dependency loading and framework targeting issues - contributions to
fix these issues would be very welcome! An updated Beta has been released as version 3.12.0-beta2.

Code contributions in this release were included from [Charlie Poole](https://github.com/CharliePoole), [Chris Maddock](https://github.com/ChrisMaddock), [Christian Bay](https://github.com/tdctaz), [Eberhard Beilharz](https://github.com/ermshiperete), [Ed Ball](https://github.com/ejball), [Joseph Musser](https://github.com/jnm2), [Manohar Singh](https://github.com/mano-si), [Mattias Cavigelli](https://github.com/mcavigelli) and [Mikkel Nylander Bundgaard](https://github.com/mikkelbu). Thank you to all those who contributed both in code, and otherwise.

You can download the NUnit Console from [GitHub](https://github.com/nunit/nunit-console/releases), [NuGet](https://www.nuget.org/) or [Chocolatey](https://www.chocolatey.org/profiles/nunit.org). See the [release notes](https://docs.nunit.org/articles/nunit/release-notes/console-and-engine.html) for more information.
