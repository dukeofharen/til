### Run an "old" MSBuild project from command line

```
msbuild "path\to.csproj" /p:DeployOnBuild=true /p:WebPublishMethod=Package /p:PackageAsSingleFile=true /p:SkipInvalidConfigurations=true /p:PackageLocation="dist" /p:Configuration=Release
```