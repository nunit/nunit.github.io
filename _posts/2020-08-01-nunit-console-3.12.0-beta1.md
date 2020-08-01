---
layout: post
title:  "NUnit Console and Engine 3.12.0 Beta 1 Released"
date:   2020-02-15 12:00:00 -0000
categories: news update nunit
---

This is the first beta release of the NUnit Console able to run .NET Core Tests. In addition to this, this release also contains a number of bug fixes, improvements when running on Mono and significant refactoring work towards the goal of creating an engine able to run tests on a wider range of .NET platforms.

We're particularly interested in this beta release being tested by users of the .NET Core console and users running tests on Mono. Please feedback any issues to the [nunit-console repository](https://github.com/nunit/nunit-console/issues).

The .NET Core Console is a separate executable to the original version, and can be found in either the .zip file download, or the new [NUnit.Console-Runner.NetCore](https://www.nuget.org/packages/NUnit.Console-Runner.NetCore/) NuGet package. Our longer-term aim is to create a single console which is able to run both .NET Core and .NET Framework tests.

Code contributions in this release were included from [Charlie Poole](https://github.com/CharliePoole), [Chris Maddock](https://github.com/ChrisMaddock), [Christian Bay](https://github.com/tdctaz), [Eberhard Beilharz](https://github.com/ermshiperete), [Joseph Musser](https://github.com/jnm2), [Manohar Singh](https://github.com/mano-si) and [Mikkel Nylander Bundgaard](https://github.com/mikkelbu). Thank you to all those who contributed both in code, and other ways!

You can download the NUnit Console from [GitHub](https://github.com/nunit/nunit-console/releases), [NuGet](https://www.nuget.org/) or [Chocolatey](https://www.chocolatey.org/profiles/nunit.org). See the [release notes](https://docs.nunit.org/articles/nunit/release-notes/console-and-engine.html) for more information.
