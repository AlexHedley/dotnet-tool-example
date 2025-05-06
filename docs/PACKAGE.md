# Package

NuGet Package Explorer
- https://apps.microsoft.com/detail/9wzdncrdmdm3?hl=en-gb&gl=US

!["NuGet Package Explorer"](images/NuGet_Package_Explorer.png "NuGet Package Explorer")

NuGet documentation
- https://learn.microsoft.com/en-us/nuget/

Package creation workflow
- https://learn.microsoft.com/en-us/nuget/create-packages/overview-and-workflow

---

Initial Properties

- [microsoft.botsay.csproj](src/microsoft.botsay/microsoft.botsay.csproj)

!["NuGet Package Explorer"](images/NuGet_Package_Explorer-1.png "NuGet Package Explorer")

Added `PackageId`, `Version`, `Authors`, `Company` and `Product`

!["NuGet Package Explorer"](images/NuGet_Package_Explorer-2.png "NuGet Package Explorer")

Added `PackageTags` and `Description`

!["NuGet Package Explorer"](images/NuGet_Package_Explorer-3.png "NuGet Package Explorer")

## Icon

https://github.com/NuGet/Home/wiki/Packaging-Icon-within-the-nupkg

```xml
<PackageIcon>icon.png</PackageIcon>
```

```xml
<ItemGroup>
  ...
  <None Include="images\icon.png" Pack="true" PackagePath=""/>
  ...
</ItemGroup>
```

Use https://mod-dotnet-bot.net/gallery/

![.NET Bot](images/dotNET-bot_kamckinn_v2.png ".NET Bot")

> Size recommendation - 128x128 (on nuget.org we use a max of 76.5x76.5 and in VS 32x32)

!["NuGet Package Explorer"](images/NuGet_Package_Explorer-4.png "NuGet Package Explorer")

## Readme

https://github.com/NuGet/Home/wiki/Embedding-and-displaying-NuGet-READMEs

```xml
<PropertyGroup>
    <PackageReadmeFile>readme.md</PackageReadmeFile>
</PropertyGroup>
```

```xml
<ItemGroup>
    <None Include="..\assets\README.md" Pack="true" PackagePath=""/>
</ItemGroup>
```

!["NuGet Package Explorer"](images/NuGet_Package_Explorer-5.png "NuGet Package Explorer")

---

# VS

![VS](images/nuget-package-properties-1.png "VS")
![VS](images/nuget-package-properties-2.png "VS")
![VS](images/nuget-package-properties-3.png "VS")

---

## Others

!["NuGet Package Explorer"](images/NuGet_Package_Explorer-6.png "NuGet Package Explorer")

- requireLicenseAcceptance
- projectUrl
- licenseUrl `<license type="expression">MIT</license>`
- repository
- copyright ?
