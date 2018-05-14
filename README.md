# ReactES6.Web

https://www.nuget.org/packages/ReactES6.Web/

---

### TL;DR

```bash
> dotnet new -i ReactES6.Web
> dotnet new reactes6 -n NewSite.Web
> cd NewSite.Web
> dotnet restore && npm install
> dotnet run
> code .
```

---

### How to Install & Run

Install the template `ReactES6.Web` from Nuget.

```bash
dotnet new -i ReactES6.Web
```

And you will see a new template named `ASP.NET Core with React.js with ES6` (with shortname _reactes6_) would appear.

```bash
dance2die@CC C:\misc\sources\throwaway\coretemplates\fromnuget
> dotnet new -i ReactES6.Web
Getting ready...
  ...

Templates                                         Short Name       Language          Tags
--------------------------------------------------------------------------------------------------------
Console Application                               console          [C#], F#, VB      Common/Console
...
ASP.NET Core with React.js with ES6               reactes6         [C#]              Web/MVC/SPA
...
ASP.NET Core with React.js                        react            [C#]              Web/MVC/SPA
ASP.NET Core with React.js and Redux              reactredux       [C#]              Web/MVC/SPA
...
MVC ViewStart                                     viewstart                          Web/ASP.NET
```

Create a new website using the template `reactes6`

```bash
dance2die@CC C:\misc\sources\throwaway\coretemplates\fromnuget
> dotnet new reactes6 -n NewSite.Web
The template "ASP.NET Core with React.js with ES6" was created successfully.
```

Go to the new website directory

```bash
cd NewSite.Web
```

Then create restore .NET Core packages and install NPM packages

```bash
dance2die@CC C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web
> dotnet restore && npm install
  Restoring packages for C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web\NewSite.Web.csproj...
  Restore completed in 140.27 ms for C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web\NewSite.Web.csproj.
  Generating MSBuild file C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web\obj\NewSite.Web.csproj.nuget.g.props.
  Generating MSBuild file C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web\obj\NewSite.Web.csproj.nuget.g.targets.
  Restore completed in 6.11 sec for C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web\NewSite.Web.csproj.
npm WARN optional SKIPPING OPTIONAL DEPENDENCY: fsevents@1.1.3 (node_modules\fsevents):
npm WARN notsup SKIPPING OPTIONAL DEPENDENCY: Unsupported platform for fsevents@1.1.3: wanted {"os":"darwin","arch":"any"} (current: {"os":"win32","arch":"x64"})

added 611 packages from 525 contributors in 95.097s
```

Start the project with `dotnet run`.

```bash
dance2die@CC C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web
> dotnet run
Using launch settings from C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web\Properties\launchSettings.json...
info: Microsoft.AspNetCore.DataProtection.KeyManagement.XmlKeyManager[0]
      User profile is available. Using 'C:\Users\dance2die\AppData\Local\ASP.NET\DataProtection-Keys' as key repository and Windows DPAPI to encrypt keys at rest.
Hosting environment: Development
Content root path: C:\misc\sources\throwaway\coretemplates\fromnuget\NewSite.Web
Now listening on: http://localhost:60672
Application started. Press Ctrl+C to shut down.
```

Open an editor of your choice (I am using VS Code below).
And play around with HMR (Hot Module Replacement) like a boss ??.

![HMR demo](https://i.imgur.com/Rbo51jW.gif)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdance2die%2FReactES6.Web.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdance2die%2FReactES6.Web?ref=badge_shield)

---

### Change Log

* v0.0.4 - Removed following folders from nupkg file.
  * bin
  * obj
  * .vscode

---

### TO DOs

1.  Automatically run `dotnet restore` upon project creation


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdance2die%2FReactES6.Web.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdance2die%2FReactES6.Web?ref=badge_large)