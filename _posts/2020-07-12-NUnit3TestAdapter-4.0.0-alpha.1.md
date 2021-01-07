# NUnit3TestAdapter version 4.0.0-alpha.1 is released.

This is an early pre-release version.

The code has been rewritten/refactored in order to get some of the more complex issues fixed. It does pass all the automatic tests we have, but there are still more tests we would like to take it through, before we release a beta.

We would really appreciate it if you give this alpha a spin. and report whatever you find back to us.

The major fix in this release is to bring back the **Explicit** test runs, both in Visual Studio and on the command line with dotnet test and vstest.console. In addition to this, the implementation handles even more cases than before.

Furthermore, there has been a significant performance improvement for large test sets, in particular when you run with categories or other filters.

## Reason for major version change

The reason for the major version change is that the way v4 interacts with the nunit.engine has been completely rewritten. The v3 version is heavily dependent on using XML internally all over the adapter code.

In v4 this has changed to transforming the xml to an object model at the time it is loaded from the engine, and then working on the object model instead. This brings back the **Explicit** feature, and the intention is to pave the way for other changes we can do. Further, under discussion is a possible drop of supporting the vsix variant, and also set the minum supported framework version to 4.5. Due to the internal rewrite there might be a intermittent loss of some features, we got one in the alpha.1 version, which is fixed now for the beta, but there might me more. However, there are around 20000 downloads now, with very few issues reported, so it might be better then feared. The changes will also pave the way for a possible better handling of the FQN issues we have - which are very annoying, and which are near impossible to handle in v3. We still need some more from MS in order to do this, but v4 should then be able to handle it. When the adapter was first written back in 2011/2012 it was a much simpler "thing" than it has become over the years. At that time the XML approach was ok, but now, the code is simply too cluttered to continue.

About the benefits in v4, in addition to bringing back the Explicit feature (and better than it was before), v4 is generally faster, and will handle large amount of tests much better. Further, with an upcoming fix in NUnit itself we can skip the pre-execution discovery phase completely, thus making the adapter even faster. This will not be possible to do with the v3 code base.
  
See [the release notes](https://docs.nunit.org/articles/vs-test-adapter/Adapter-Release-Notes.html#nunit3-test-adapter-for-visual-studio---version-400-alpha1---july-12-2020) for details on what has changed in 4.0.0-alpha.1.  
[Download NuGet package](https://www.nuget.org/packages/NUnit3TestAdapter/4.0.0-alpha.1)

Note:  There is no VSIX for pre-releases since that is not supported by the VSIX system. 
