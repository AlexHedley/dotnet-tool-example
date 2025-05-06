# Docs

## Articles

- Tutorial: Create a .NET tool using the .NET CLI
  - https://learn.microsoft.com/en-us/dotnet/core/tools/global-tools-how-to-create

```bash
dotnet new console -n microsoft.botsay -f net9.0
```

Add code

Update `.csproj`

```bash
dotnet pack
```

- Tutorial: Install and use a .NET global tool using the .NET CLI
  - https://learn.microsoft.com/en-us/dotnet/core/tools/global-tools-how-to-use

```bash
dotnet tool install --global --add-source ./nupkg microsoft.botsay
```

> You can invoke the tool using the following command: botsay
> Tool 'microsoft.botsay' (version '1.0.0') was successfully installed.

```bash
botsay hello from the bot
```

```bash
dotnet tool uninstall -g microsoft.botsay
```

> Tool 'microsoft.botsay' (version '1.0.0') was successfully uninstalled.

- Tutorial: Install and use a .NET local tool using the .NET CLI
  - https://learn.microsoft.com/en-us/dotnet/core/tools/local-tools-how-to-use

```bash
cd ..
```

```bash
dotnet new tool-manifest
```

> The template "Dotnet local tool manifest file" was created successfully.

```bash
dotnet tool install --add-source ./microsoft.botsay/nupkg microsoft.botsay
```

> You can invoke the tool from this directory using the following command:  
> 'dotnet tool run botsay' or 'dotnet botsay'  
> Tool 'microsoft.botsay' (version '1.0.0') was successfully installed.  
> Entry is added to the manifest file /home/name/repository/.config/dotnet-tools.json

- [dotnet-tools.json](../src/.config/dotnet-tools.json)

Use

```bash
dotnet tool run botsay hello from the bot
```

Restore 

```bash
dotnet tool list
```

```bash
Package Id            Version      Commands      Manifest
----------------------------------------------------------------------------------
microsoft.botsay      1.0.0        botsay        ...\src\.config\dotnet-tools.json
```

Update

```bash
dotnet tool update dotnetsay
```

Remove

```bash
dotnet tool uninstall microsoft.botsay
```

```bash
dotnet tool uninstall dotnetsay
```
