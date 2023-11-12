| [Home](../../README.md) | [Targets](README.md) |

<hr style="height: 1px" />

# MSBuild Target "CompileWindowsResource"

This target compiles a Windows Resource Script (\*.rc) file into it's Windows
Resource file (\*.res). The target uses the [(Windows) Resource Compiler (RC)](https://learn.microsoft.com/en-us/windows/win32/menurc/resource-compiler)
(`rc.exe`). It requires the build property `RCToolPath` which must point to
the full path of that tool from build tools, Windows SDK or Windows Kit's and
the build property `WindowsResourceFileName` which must point to the relative
path to the Windows Resource Script file from the base of `ProjectDir`. The
target computes then the `WindowsResourceFilePath` build property from `ProjectDir`
and `WindowsResourceFileName`. The build properties could be added at the project
file, `Directory.Build.props`, `Directory.Build.targets` or any other properties
or target(s) file.



## Locations of (Windows) Resource Compiler (rc.exe)

```
C:\Program Files (x86)\Windows Kits\<VersionMajor>\bin\<Version>\x86\rc.exe  
C:\Program Files (x86)\Microsoft Visual Studio\Shared\NuGetPackages\microsoft.windows.sdk.buildtools\<RevisionVersion>\bin\<Version>\x86\rc.exe
C:\Program Files (x86)\Microsoft Visual Studio\Shared\NuGetPackages\microsoft.windows.sdk.buildtools\<RevisionVersion>\bin\<Version>\x64\rc.exe
```

Windows SDK BuildTools can obtained from nuget.org ([Microsoft.Windows.SDK.BuildTools](https://www.nuget.org/packages/Microsoft.Windows.SDK.BuildTools/)).



## Errors

- When build property `RCToolPath` is not set
- When file from build property `RCToolPath` target not found
- When build property `WindowsResourceFileName` is not set
- When file from build property `WindowsResourceFilePath` target not found



<!-- FOOTER -->
<hr style="height: 1px" />
<span style="font-size: 0.7em">© SphereSoft.NET, Holger Boskugel, Berlin, Germany</span>
<a href="http://spheresoft.net" style="font-size: 0.7em; float: right">spheresoft.net</a>
