| [Home](../../README.md) | [Targets](README.md) |

<hr style="height: 1px" />

# MSBuild Target "TargetFrameworkVersionPreprocessorSymbols"

This target creates preprocessor constants for the target .NET Framework like
Microsoft has introduced it to .NET (Core) ([Target frameworks in SDK-style projects
\- Preprocessor symbols](https://learn.microsoft.com/en-us/dotnet/standard/frameworks#preprocessor-symbols)).
In general the constant `NETFRAMEWORK` will be added and the version related
constant from this list:

| Version | Constant |
| --- | --- |
| v4.8   | NET48  |
| v4.7.1 | NET471 |
| v4.7   | NET47  |
| v4.6.2 | NET462 |
| v4.6.1 | NET461 |
| v4.6   | NET46  |
| v4.5.2 | NET452 |
| v4.5.1 | NET451 |
| v4.5   | NET45  |
| v4.0   | NET40  |
| v3.5   | NET35  |
| v3.0   | NET30  |
| v2.0   | NET20  |
| v1.1   | NET11  |



<!-- FOOTER -->
<hr style="height: 1px" />
<span style="font-size: 0.7em">© SphereSoft.NET, Holger Boskugel, Berlin, Germany</span>
<a href="http://spheresoft.net" style="font-size: 0.7em; float: right">spheresoft.net</a>
