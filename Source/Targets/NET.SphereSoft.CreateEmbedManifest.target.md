| [Home](../../README.md) | [Targets](README.md) |

<hr style="height: 1px" />

# MSBuild Target "CreateEmbedManifest"

This target creates a COM (ActiveX) manifest from the target output and embeds
it there. The target uses the [MT](https://learn.microsoft.com/en-us/windows/win32/sbscs/mt-exe)
(`mt.exe`) tool for creation and embedding. It requires the build property
`MTToolPath` which must point to the full path of that tool from build tools,
Windows SDK or Windows Kit's. The build property could be added at the project
file, `Directory.Build.props`, `Directory.Build.targets` or any other target.



## Errors

- When build property `MTToolPath` is not set
- When file from build property `MTToolPath` target not found



<!-- FOOTER -->
<hr style="height: 1px" />
<span style="font-size: 0.7em">© SphereSoft.NET, Holger Boskugel, Berlin, Germany</span>
<a href="http://spheresoft.net" style="font-size: 0.7em; float: right">spheresoft.net</a>
