NUnit3TestAdapter version 3.15.1 is released.

This is a hotfix release.  
Vesion 3.15.0 introduced a prefilter to increase VS test performance.  In a few cases, see  [Issue 651](https://github.com/nunit/nunit3-vs-adapter/issues/651) which also contains links to the different cases, the tests was not run.  One of the issues is also caused by an [NUnit Framework issue](https://github.com/nunit/nunit/issues/3356). 

In this hotfix the prefilter is behind a feature flag, which by default is off. It can be turned on by setting a [PreFilter option in a runsettings](https://github.com/nunit/docs/wiki/Tips-And-Tricks#PreFilter) file. 
  
See [the release notes](https://github.com/nunit/docs/wiki/Adapter-Release-Notes) for details on what has changed in 3.15.1  
[Download NuGet package](https://www.nuget.org/packages/NUnit3TestAdapter/3.15.1)
[Download VSIX](https://marketplace.visualstudio.com/items?itemName=NUnitDevelopers.NUnit3TestAdapter)