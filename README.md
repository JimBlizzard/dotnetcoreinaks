# This is my journey to create a dotnet core app and stuff it into AKS. Properly.

The App is based on [MiniBlog.Core by Mads Kristensen](https://github.com/madskristensen/Miniblog.Core)

For now I'll document my efforts along the way, here in the MD file. Once I get the engine up & running in AKS I'll start documenting things there. 

## prerequisites

I installed Ubuntu in WSL (Windows Subsystem for Linux) on Windows 10. 
https://docs.microsoft.com/en-us/windows/wsl/install-win10

I also installed [Docker Desktop](https://docs.docker.com/docker-for-windows/install/). It includes the Docker Engine, Cli client, Kubernetes, etc. 

For this effort I'm using Linux containers, not Windows Containers.

## the app
I cloned the Miniblog.Core repo from  https://github.com/madskristensen/Miniblog.Core.git

