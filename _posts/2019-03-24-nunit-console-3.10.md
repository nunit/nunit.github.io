---
layout: post
title:  "NUnit Console and Engine 3.10 Released"
date:   2019-03-24 12:00:00 -0000
categories: news update nunit
---
This release merges the .NET Standard version of the engine back into the nunit.engine NuGet package and adds a .NET Standard 2.0 version of the engine that re-enables most services and extensions. This deprecates the `nunit.engine.netstandard` NuGet package. Any test runners using the old .NET Standard version of the engine should switch to this release.

The --params command line option which took multiple test parameters separated by a semicolon is now deprecated in favor of the new --testparam command line option. One of the most common uses for test parameters was to pass connection strings into tests but this required workarounds to handle the semicolons. Now you must pass in each test paramater separately using a --testparam or --tp option for each.

You may download NUnit Console 3.10 from [Github](https://github.com/nunit/nunit-console/releases). See the [release notes](https://github.com/nunit/docs/wiki/Console-Release-Notes) for more information.