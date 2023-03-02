# Exemplo.Package

comandos para criar o package e fazer o push

```
dotnet nuget add source https://nuget.pkg.github.com/<USUARIO DO SEU GITHUB>/index.json
dotnet build --configuration Release
dotnet pack --configuration Release
dotnet nuget push "./bin/Release/Exemplo.Package.1.0.0.nupkg" -k <TOKEN DO SEU GITHUB> -s https://nuget.pkg.github.com/<USUARIO DO SEU GITHUB>/index.json
```

comando para limpar o cache local do nuget

```
dotnet nuget locals all --clear
```
