| [Home](../../README.md) | [Targets](README.md) |

<hr style="height: 1px" />

# MSBuild Target "TransformXmlAppConfig"

This target transforms the XML of app.config file based on templates.

See Microsoft articles

- [Transform web.config](https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/transform-webconfig)
- [Web.config Transformation Syntax for Web Application Project Deployment](https://learn.microsoft.com/en-us/previous-versions/dd465326)
- [Web.config Transformation Syntax for Web Project Deployment Using Visual Studio](https://learn.microsoft.com/en-us/previous-versions/aspnet/dd465326)

for concept an syntax also.



## Process

- Apply transformation of configuration "Debug" (`app.Debug.config`) if exists
- Apply transformation of configuration and computer (`app.<Configuration>.<COMPUTERNAME>.config`)
  if exists
- Apply transformation of configuration (`app.<Configuration>.config`)
  if exists and no template for configuration and computer exists (`app.<Configuration>.<COMPUTERNAME>.config`)



<!-- FOOTER -->
<hr style="height: 1px" />
<span style="font-size: 0.7em">© SphereSoft.NET, Holger Boskugel, Berlin, Germany</span>
<a href="http://spheresoft.net" style="font-size: 0.7em; float: right">spheresoft.net</a>
