---
layout: post
title:  "NUnit Console and Engine 3.9 Released"
date:   2018-09-05 12:00:00 -0000
categories: news update nunit
---
This release should stop the dreaded SocketException problem on shutdown. The console also no longer returns -5 when AppDomains fail to unload at the end of a test run. These fixes should make CI runs much more stable and predictible.

For developers working on the NUnit Console and Engine project, Visual Studio 2017 update 5 or newer is now required to compile on the command line. This does not effect developers using NUnit or the NUnit Console, both of which support building and running your tests in any IDE and on any .NET Framework back to .NET 2.0.

You may download NUnit Console 3.9 from [Github](https://github.com/nunit/nunit-console/releases). See the [release notes](https://github.com/nunit/docs/wiki/Console-Release-Notes) for more information.