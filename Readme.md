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