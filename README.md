# aspcore-on-linux
Sample app running on Linux on WSL

To create and publish the app run fallowing two commands:
```bash
dotnet new webapp -n SelfContainedAspCoreOnLinux
```

```bash
dotnet publish -r linux-x64 -c Release /p:PublishSingleFile=true /p:PublishTrimmed=true
```
Next switch to WSL and run selfcontained executable!:
```Bash
bash
./SelfContainedAspCoreOnLinux
```