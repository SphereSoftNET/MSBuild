| [Home](../../README.md) | [Targets](README.md) |

<hr style="height: 1px" />

# MSBuild Target "CreateEmbedManifest"

This target creates a COM (ActiveX) manifest file (\*.mainfest) from the target
output and embeds it into the target output. The target uses the [Manifest Tool (MT)](https://learn.microsoft.com/en-us/windows/win32/sbscs/mt-exe)
(`mt.exe`) for creation and embedding. It requires the build property
`MTToolPath` which must point to the full path of that tool from build tools,
Windows SDK or Windows Kit's. The build property could be added at the project
file, `Directory.Build.props`, `Directory.Build.targets` or any other properties
or target(s) file.



## Locations of Manifest Tool (mt.exe)

```
C:\Program Files (x86)\Windows Kits\<VersionMajor>\bin\<Version>\x86\mt.exe  
C:\Program Files (x86)\Microsoft Visual Studio\Shared\NuGetPackages\microsoft.windows.sdk.buildtools\<RevisionVersion>\bin\<Version>\x86\mt.exe
C:\Program Files (x86)\Microsoft Visual Studio\Shared\NuGetPackages\microsoft.windows.sdk.buildtools\<RevisionVersion>\bin\<Version>\x64\mt.exe
```

Windows SDK BuildTools can obtained from nuget.org ([Microsoft.Windows.SDK.BuildTools](https://www.nuget.org/packages/Microsoft.Windows.SDK.BuildTools/)).



## Errors

- When build property `MTToolPath` is not set
- When file from build property `MTToolPath` target not found



<!-- FOOTER -->
<hr style="height: 1px" />
<span style="font-size: 0.7em">© SphereSoft.NET, Holger Boskugel, Berlin, Germany</span>
<a href="http://spheresoft.net" style="font-size: 0.7em; float: right">spheresoft.net</a>
