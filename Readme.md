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