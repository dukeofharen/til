### Use latest language version
```
<LangVersion>latest</LangVersion>
```

### Use full .pdb debugging
```
<PropertyGroup Condition=" '$(Configuration)' == 'Debug' ">
  <DebugType>Full</DebugType>
</PropertyGroup>
```