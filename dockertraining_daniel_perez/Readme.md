# Assignment for Docker in Visual Studio

## Commands

```powershell
docker build -f "C:\Workspace\Training\docker-training\Code\dockertraining_daniel_perez\Dockerfile" --force-rm -t dockertraining_daniel_perez  "C:\Workspace\Training\docker-training\Code" 

docker run --name Site1 -p 8085:80 dockertraining_daniel_perez

docker run --name Site2 -p 8086:80 -e "AppSettings:storename"="Plano" dockertraining_daniel_perez

docker run --name SiteQA -p 8086:80 -e "AppSettings:storename"="Plano" -e "AppSettings:environment"="QA" dockertraining_daniel_perez

docker run --name SiteUAT -p 8086:80 -e "AppSettings:storename"="Plano" -e "AppSettings:environment"="UAT" dockertraining_daniel_perez

docker run --name SitePROD -p 8086:80 -e "AppSettings:storename"="Plano" -e "AppSettings:environment"="PRODUCTION" dockertraining_daniel_perez

```



