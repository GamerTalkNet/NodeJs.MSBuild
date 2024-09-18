## GamerTalk.NodeJs.MSBuild

This package allows you to have Node.Js packages as dependencies within your .NET projects.

To use this simply install the package using your IDE or from the command line with the command below:
```batch
   dotnet install GamerTalk.NodeJs.MSBuild --prerelease
```

Then reference your required packages as NodePackageReference in your project as shown in the example below:
```xml
<ItemGroup>
    <NodePackageReference Include="typescript" />
</ItemGroup>
```
Or, if you would like to specify the version.
```xml
<ItemGroup>
    <NodePackageReference Include="typescript" Version="5.5.3" />
</ItemGroup>
```

### TODO
- [x] Add method to install Node.Js packages.
- [x] Add way to specify package version.
- [ ] Add check for current version to update/downgrade to specified version.
- [ ] Add metadata option to specify the type of dependency (normal, development, embedded, optional).
