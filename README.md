# B9MG119-Assignment

## Company Choosen: Thryve Digital

![alt text](https://fresheropenings.com/wp-content/uploads/2022/09/Thryve-Digital-Off-Campus-Drive-for-2022-Batch.png)
### **INTRODUCTION**
____________________
Business right now started to hire larger number of technical persons as fresher and expereience candidates. HR team having lots of works which needs to be organized effectively so the recruitement process would be seemless. For this, the team looking for a todo list which help them to organzie their day today job. HR team also conduct on-campus drive so the todo list should not only be in their local machine. It should be reached from anywhere when HR team requires. Since the recruitement process having lots of confidential information, the what ever data entered with in the application should stored in secured manner. Keeping everything in a personal computer or laptop is not an idle case in this requirement. So the todo application should hosted in a secured server. On-permisis option is too costly which require a technical person support to provision the server, internet connection, uninterupted powersupply to server. Licenses includes operating system, Databases, and other tools also plays a vital role. Off campus drives are happening only at the education year end. Moving the application to cloud helps to avoid the major cost which stated above and also once drive completed we can decrease the resource usage which helps to cut down the cost.
## Benefits of cloud 
_____________________
-Easy to provision - We no need to worry about purchase servers, required Licenses for softwares and etc. All can be done in matter of minute.
-Easy to scale - When require the system can be scaled up/down depends upon the specific requirement.
-Cost Effective - We are going to pay as we use. So no additional cost incurred.
-Security - On security aspects, firewall, os patch and etc handled by cloud infrastructure which increase the security without much intervention.
![alt text](https://iamguptarishi.files.wordpress.com/2019/03/3-azure-services.png)
## **Background Of The Enterprise**
___________________________________
The company is founded in India and providing healthcare releated IT services to different countries. Their primary focus is on IT enabled services to their overseas clients. They are offering services included Information technology health plan solutions, Information technology health customer solutions, Applicaitons and platform management.
### Current IT Set Up
______________________
The system is currently installed in an on-premises infrastructure.There are moret tha 500 people working on the organization. They are employing peoples who can serve healthcare related solutions to their customers. There are certain cloud virtual machine technologies. Essentially, They are creating everything in a private Virtual machine environment and have picked Azure as their cloud service provider.
## Contrast of cloud and non-cloud solutions 
--------------------------------------------
The services offered by the cloud vendor always have an impact on the deployment architecture of a cloud-ready application. The choice of cloud services becomes even more crucial for an application that must operate under strict compliance and data residency requirements. Also in cloud vps they are using Docker images to deploy the application which helps to keep the application deployment in an effective manner without worrying about tools and supporting frameworks.
### Cloud
_________
- Improved forecasting and management of costs.
- Integrated disaster recovery and enhanced backup and restoration.
- Higher scaleability.
- Updates to applications such as operating system, databases are automated.
- Physical firewall setup and configuration.
- Docker image support with server and serverless environment.
- Can deploy almost any type of application without worrying about operating systems (Windows/Linux).
### Non-Cloud 
_____________
- Within the same data center or in office permisis.
- High levels of security and discretion. Require system administrator who requires to keep an eye on almost everything.
- Maintenance including internet redudency, uninteruppted powersupply is challenging.
- Performing the backups in manual way. If it automated using any additional softwares, then the license cost also added with expenses.
- Most of the license can not be leased hence we need to pay full money.

### Docker support
___________________
Docker allows us to package our application and deliver them to cloud without any dependencies. The Docker platform allow us to run our application in an isolated environment and allow us to automatically scale up or scale down. The docker is idle way to deliver application which does not having dependency. For example the company can able to run the Todo application in a separate container under virtual machine which already running a accounting software under it as separate container. Both can have their own dependency. For example one application requires python and another one runs on .net core. The docker having following benifits
- Flexible resource sharing - includes capacity of server resources such as ram, processing power and etc
- Scalablity - When requires we can scale up or scale down a particular container.
- Cost Effective - Running services on hardware is much cheaper than standard server.
- Fast deployment - Bundle always having supporting dependencies. So deployment is seemless.
- Easy of migration - We can migrate the application to another location easily.
- Better Security - Less access to work with the code running inside containers. Fewer software dependencies.
## Cloud architecture deployment proposed
_________________________________________
The proposed architecture which includes from developing, maintaining application to deployment of the applicaiton. For development purpose the company use free applications such as VSCode for code development. For better code maintanance the proposed system includes a SVN system from Github. The github act as code repository which helps developer to track their changes and keep the code clean and effective.

Since the company uses private virtual machines for their data security purpose, the application also having docker image configuration, which also created and maintained as part of code repository.

For continious development of the application and deployment, Azure devops recommened. Azure devops helps to compile the source code and deliver the build to the azure environment via pipelines.

For virtual machine front, linux flavor recommended to keep the cost low.

- Git Repository - The application uses Git for code repository. The code repository also contains docker configuration.
- Azure DevOps - Build pipeline - The application build via private build pipeline. Microsoft provide free hours for building private repositories. Since the application not going to change time to time, free hours are enough.
- Azure Devops - Release pipeline - To deliver the docker image to cloud Azure release pipeline helps.
- Docker image - The docker image configuration is part of Git code repository. The build pipeline will build the information and prepare the docker image.
- Virtual Machine - As a part of deployment the company created virtual machine with Linux operating system with docker support. So the devops will deploy the docker image directly to the virtual machine.

# Conclusion 
_______________ 
When comparing the cloud based solution with non-cloud based solution, the cloud based solution is much better interms of effectiveness, security, data redudency, ease of deployment at the same time keeping the cost low. Azure pricing calucator helps to forecast the cost for each month depends upon the usage. This helps to keep management aware of the expenses comes with in their budget. Also, it helps to optimize our resource usage.
## Referance 
Microsoft azure (https://azure.microsoft.com/)

Azure pricing calculator (https://azure.microsoft.com/en-in/pricing/calculator/)

Docker support (https://docs.docker.com/cloud/aci-integration/)

Docker Support - Microsoft (https://learn.microsoft.com/en-us/azure/app-service/tutorial-custom-container?tabs=azure-cli&pivots=container-linux)

Azure Devops - (https://azure.microsoft.com/en-in/products/devops)

Azure Devops - Docker support (https://learn.microsoft.com/en-us/azure/devops/pipelines/tasks/reference/docker-v2?view=azure-pipelines&tabs=yaml)
