# AZURE CLOUD SERVICES

## Describe Cloud Computing
### Shared Responsibility Model
* If we have our own **DataCenters**, then we need to responsible for all the factors such as Natural Disasters, Network, Operating System's Update, Security, Data breach, etc..
* This is our head weight only, isn't it?
* For me, i need to design **WebApplication**, and provide **good service** to my customers. These things are all **extra burden**.
* So to handOver this problems to great organizations such as `Microsoft`, Google, Amazon as a **Cloud service**, they can take over all the problems and provide good service for us.
* Here we are `sharing our Responsibility` to them.
* But eventhough we were share our responsible, still we need to handle some of the **security informations** such as our User's credential, Authentication, Application security... these thing are took care by ourself.
* So we are `mixed sharing the Responsibilities`.

![Shared Responsiblity Modle](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/bf90f2ed-793a-42ee-821a-b705fe73df6c)

![Shared Responsible with Microsoft](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/8f44f18a-564c-4dee-a815-f8e78bb69393)

### Private, Public, and Hybrid Cloud
* Public cloud is Microsoft has an own hardware and give services for everyone with the public Network, those who have credit card they can access the Public Cloud.
* Private is some organization offer some services that is only accessible by certain people and they were maintained that by private internet.
* Hybrid is the combination of both, that's all.

### Cloud Pricing
* It is difficult to predict our **Monthly Bill** on cloud.
* We can end up with one thought as, we could keep track of price for every month **(History)**.
--------
#### Factors that affect Virtual Machine Costs
![Virtual Machine](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/fcc073cb-4ff9-49e2-be99-0576ab519cfd)

### Factors that affect Cosmos DB
1. API Choice
2. Regions
3. Optional Dedicated Gateway
4. Number of Operations per second
5. Consumed Storage
6. Backup Storage

* We need to pay for the storage of our services, it is based on **Gigabytes(GB)**, how much time we are using.
* Pay for Operations, We are doing operations such as read, write, delete, update for all these, they charged in a **little amount**. Pay per message, Pay per query to a database...

## Describe Benefits of Cloud Computing
### High Availability benefit of cloud computing
* Even if the situation is too bad, planned and unplanned outages, services should be available to operate. That company having the High Availability.

#### Planned Outages
1. Hardware Replacement
2. Deployment (Application updates)
3. Migrating to new hosting provider
4. Operating system security patches

#### Unplanned Outages
1. Natural Disasters
2. Human Disasters (Cyber attacks)
3. Power outages
4. Stable Network connection
5. Hardware failure
6. Software bugs
7. Poor scaling or architecture design

### Scalability of Cloud Computing
* By adding or removing of certain resources, our system needs to give **great performance**.
* This scaling involves to handle the `traffic` in the system, but traffic is always fluctuate depends on day.
* **E-commerce** website have `Black Friday`, that time they reboot their system and control the traffic.
* Like School registrations are busy at June, and Tax systems are buys in April. During these time traffics are busy.

#### Vertical Scaling
* Scaling-up or Scaling-down.
* We could add more number of resources on a single server.
* But it has upper limit for Azure, 96 CPUs and 384 GB of memory.

#### Horizontal Scaling
* Scaling-out or Scaling-in.
* We could add more servers itself to the system.
* There is no limits
* But it has increase complexities in load balancing.

### Elasticity of Cloud Computing (Auto-Scaling)
* Instead of static capacity of system, it will **dynamically grows and shrinks** according to the `User demand`.
* So, our system can able to utilize the **waste resources** also.

### Reliability of Cloud Computing
* All these Availability, Reliability and Predictability are there to **provide the solution** for the common problem and give **high quality services** to the customers.
* `Reliability is, the system is intented to perform particular function without interruption and with a higt degree of accuracy.`
* Without Reliability, **availability** is waste of thing, because availability in the sense, our system is doing work while all scenarios are outages, but what if our system itself perform in a wrong way instead of what we expect.

#### Availability Vs Reliability
* Availability is an appearance to end users.
* Reliability is the underlying truth.
------
* This includes **Transparency** during service issue.

### Predictability
* Our system will able to **predict** how customer's Application should be perform, and how much cost it needed for Cloud, like all the required things should able to give priorily.
* I hosted my application on Azure for one week, then Azure should be *capable to predicting* how much cost, I need to pay after one month, one year, and how my application will perform, etc...

### Security of Cloud Computing
* Giving security to the cloud is one of the important things to the provider.
* Microsoft and other Big Organizations are invest their Money, Time and effort for Security. Security is the first preference to them.
* They are very conscious about the hackers, and protect our data (billions of people's data), implementing TLS(Transport Layer Security) and some other ideas.
* Microsoft's Security Preventions:
    1. Industry Standard Compliance Certificates (ISO)
    2. Microsoft Security Response Centres (MSRC)
    3. Always on `DDoS` (Distributed Denial of Services) => One user requesting one server, but attackers give floods of request to the server, then server got crashed. So Microsoft are ready to prevent these attacks too.
    4. Role Based Access Control (RBAC)
    5. Azure Active Directory
    6. Always up-to date platform services
    7. Encryption **By default**
    8. Dozens of Security Services like `Firewall`

### Governance
* How a Organization `does a Business`.
* How they were defining, implementing, and Monitoring the Framework policies.
* Organizations needs to ensure all Policies, and follows **HIPAA**(Health Insurance Portability and Acountability Act) to give quality services to the customers.
* Follows Azure Policies and Blueprint.
* Custom Roles (RBAC)
* Soft Deletes => save data for certain period of time from Accidental delete.
* Guides and Best practices such as **Cloud Adoption Framework**.

## Cloud Service Types
1. IaaS - Infrastructure As a Service
2. PaaS - Platform As a Service
3. SaaS - Software As a Service

> `As a Service?` => Instead of Owing a particular service, we can just took a **rent** on them. Pay for what you use. Cloud Providers could take care all the underlying properties such as buying, developing, maintaining, security, etc..

## Azure Architecture and Services
### Regions
* Microsoft Azure's Datacenters are spreaded all over the world through `Regions`.
* There are `60+` Regions are there, each Region have mininum **Three data centers** in it.
* Most of the countries have **Paired Regions**, which involves fastest connection and pairs have Backup Datas, if any massive transfer wants to happen, that can achieve through **Region Pairs**.
* **Light grey colour dot** in the Map represents, Data Centers is going to `coming soon`.

![Canada Region](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/7de89a25-e687-48a4-9468-66d7aa4383c8)

![Brazil Region](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/d6dd70c8-36b9-4f66-937e-e66f3436639b)

![Qatar Region](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/4c1d3ecb-dc05-4a71-861d-d6059744b743)

![Region Pairs](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/88ac15d5-04e7-47e5-aa6c-94a79e0beef2)

* Not all 60+ regions are available to everyone, if we want then we have to the **local resident** of that Region or We need to be joined in the `Sovereign Regions`.

#### Sovereign Regions
* Those who wants to make their data private, or countrie's government or private organizations are come under Sovereign Regions.
* They are not connected to **Public Cloud**.
* If we want to join, we need sepearate `approval or subscription`.
* We need to follow different compliance standards.

![Cloud Mission](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/835593f2-72ac-4ed4-9d8e-a3355ded46d1)

### Availability Zones
* Group of Data Centers inside the Regions are called Availability Zone, it would share Network, Security, etc...
* But **Not every Regions** supports Availability Zones.
* As well as **not every Service** supports Availability Zones, may that will resolve by updating them.
* Regions which have Availability Zones

![Availability Zone Regions](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/7f3df252-0142-4fa9-8891-7c4d57d01451)

#### Types of AZ Services
1. Zonal Services
2. Zone-Redundant Services
3. Always available Services

##### Zonal Services
* Customers wish to deploy on **which Available zone** in tha Particular Region, and they can deploy their `resource's duplicates` into other Available zone in the same Region, for safety purpose.

##### Zone-Redundant Services
* Azure itself take care of deploying our duplicates into multiple Availability Zones.

##### Always Available Services
* There is one Global Service or Region, that was handled by Azure, if others goes down, it still remains.

### Resources and Resource Groups

![Resource](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/fb60ae61-84be-4452-af8b-938d1a8373e1)

* **Resources** are the services provide by Azure, that we can create for our purpose by Azure portal, CLI, Scirpts, etc...
* We could deploy these Resources at our **preferred location or Regions**.
* Resource groups are consists of group of Resources, it could have **resources from different Regions** also.
* But the Resources inside the Resource Group should have `similar relations` such as deploy together, delete together.
* One Resource should map to only one Resource Group.
* `Permissions` (Read or Write) can be assigned to the Resource Group level.
* But we could not create **intra Azure permissions** for the Resource to communicate with each other.

### Subscriptions
* Subscription is `Billing Unit` and Resource Groups are grouped under a single Subscriptions.
* One can have **Multiple Subscriptions** and it would map with any payment type, like Credit card.
* Subscription Plans in Azure

![Subscription Plans](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/433feb52-356d-4197-a8e0-400e7e59b536)

* A Company's Subscription Strategy

![Subscription Strategy](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/0a45721e-527e-4854-bfa7-4a016c75c20c)

> But a Company can operate in a **Single Subscription** also.

* All Subscriptions are grouped under a single Management Group.

## Azure Compute Services and Virtual Machines

* Four Technical Pillars of Azure Services
1. Compute Services
2. Network Services
3. Storage Services
4. Database Services

### Compute Services
* `Executing a Code on the Server`

![Computing Services](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/753b220a-a193-4535-92b4-8bccd81981a6)

#### Standalone Server Analogy
* Server can host independently without affecting other servers.
* Like a Single-detached house, we don't want disturb others but instead we can utilize common things like Water, Electricity, etc...
* Virtual Machine in AWS is Called **EC2** instance. `(Elastic Compute Cloud)`.

### Scaling Virtual Machines
* We can increase the Configurations of VMs from 4CPU to 8CPU, this is Scale Up.
* We can increase the VMs numbers also, this is Scale Out.

### App Services or Web Apps
* Our own application can able to run on the server in the Microsoft, we should package our code and configurations and deployed at the server, it can execute.
* But we don't know, the underlying properties, like how server is executing, we cannot have access to Server settings.
* Promise of Performance but no access to hardware.
* It is PaaS (Platform).

### Container Service
* Container contains everything that a application need to execute in a `Container Image`.
* Fastest and Easiest to deploy. It will automatically deploy to different environments.

![Container Service](https://github.com/rkishore1207/Cloud-Learning/assets/146698138/2ec82881-5c0c-4372-b4e7-af72c321c263)

### Azure Virtual Desktop
* It's like a our own desktop that is deployed in the Azure, that is available for different device and for different Softwares.
* Our Software installed, files can be available from anywhere.

### Virtual Network (VNet)
* It is Network which is analogy to Physical Network, but it doesn't have Cables, wires...
* By default, two Virtual Machines in Azure are not allowed to talk with each other - **Security**.
* In Azure, it's virtual because it's just an entry to the database, that establishes the path between **VM A and VM B**.
* Iaas
* While create VNet, we should be assign address space like IPv4 or IPv6 or both, after creation, if we want to increase the range, we could add extra ranges too.
* It is `Private Network`, which cannot be accessed from outside of Azure or other networks inside of Azure.

#### Subnet
* VNets are divided into **Subnets**, if we create Subnet then that address should be Present in the Parent VNet.
* All Subnet have Security Layer.
* All Subnets are connected with VMs through **NIC(Network Interface Card)**.