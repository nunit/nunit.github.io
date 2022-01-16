---
layout: post
title:  "NUnit Console and Engine 3.13 Released"
date:   2021-12-01 12:00:00 -0000
categories: news update nunit
---

This is the first release of the NUnit Console Runner, which allows running of both .NET Framework and .NET Core tests, either separately or in combination. The Console Runner executes under the .NET Framework but is able to launch .NET Core agents and communicate with them over a TCP connection.

A second major feature is the availability of preemptive cancellation when the normal approach of requesting the test run to terminate itself doesn't work. This is an engine feature, available to any runners supporting cancellation.

This release includes code contributions from [Charlie Poole](https://github.com/CharliePoole), [Joseph Musser](https://github.com/jnm2), [Mikkel Nylander Bundgaard](https://github.com/mikkelbu), [Chris Maddock](https://github.com/ChrisMaddock), [Rob Prouse](https://github.com/rprouse), [Ian144](https://github.com/ian144), [TillW](https://github.com/x789), [Manfred Brands](https://github.com/manfred-brands), [Timon](https://github.com/TimonPost) and [Sean Killeen](https://github.com/SeanKilleen). Thank you to all those who contributed both in code, and otherwise.

You can download the NUnit Console from [GitHub](https://github.com/nunit/nunit-console/releases), [NuGet](https://www.nuget.org/) or [Chocolatey](https://www.chocolatey.org/profiles/nunit.org). See the [release notes](https://docs.nunit.org/articles/nunit/release-notes/console-and-engine.html) for more information.
