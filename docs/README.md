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

