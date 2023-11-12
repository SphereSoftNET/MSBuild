| [Home](../../README.md) | [Targets](README.md) |

<hr style="height: 1px" />

# MSBuild Target "TextTemplating.T4"

This target configures the parameters and imports the [Microsoft T4 `TextTemplating`](https://learn.microsoft.com/en-us/visualstudio/modeling/code-generation-and-t4-text-templates)
targets for processing text templates (\*.tt) during build process.

It requires the installed MBuild Component `Microsoft.VisualStudio.Component.TextTemplating`.
Formerly package was known as "Modeling (And Visualization) SDK for Visual Studio".



## Template variables from MSBuild Properties

For template processing the following variables get handover to be retrievable
in MSBuild and Visual Studio builds:

- `ProjectPath`



## Errors

- When build property `MSBuildExtensionsPath32` is not set
- When build property `VisualStudioVersion` is not set
- When file from computed build property `TextTemplatingTargetsPath` target not found



<!-- FOOTER -->
<hr style="height: 1px" />
<span style="font-size: 0.7em">© SphereSoft.NET, Holger Boskugel, Berlin, Germany</span>
<a href="http://spheresoft.net" style="font-size: 0.7em; float: right">spheresoft.net</a>
