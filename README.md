# This is my journey to create a dotnet core app and stuff it into AKS. Properly.

The App is based on [MiniBlog.Core by Mads Kristensen](https://github.com/madskristensen/Miniblog.Core)

The ultimate goal is to 
1. Run Miniblog.Core safely and securely in AKS. (All proper network / security / healt checks / secrets management / yada yada yada) in place.
1. Deploy updates to the engine in AKS through GitHub CI/CD pipelines, which will include container scans, etc., using blue/green pattern. 
1. The Docker image will be stored in the Azure Container Registry.
1. And other things. . . 

For now I'll document my efforts along the way here in the MD file. Once I get the engine up & running in AKS I'll start documenting things there. 

## prerequisites

I'm running Ubuntu in WSL (Windows Subsystem for Linux) on Windows 10. 
https://docs.microsoft.com/en-us/windows/wsl/install-win10

I also have [Docker Desktop](https://docs.docker.com/docker-for-windows/install/). It includes the Docker Engine, Cli client, Kubernetes, etc. 

And I'm using Linux containers, not Windows Containers.

## the app

I cloned the Miniblog.Core repo from  https://github.com/madskristensen/Miniblog.Core.git

