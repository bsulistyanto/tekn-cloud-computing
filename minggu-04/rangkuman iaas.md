RANGKUMAN IAAS
IaaS (Infrastructure-as-a-Service)
Infrastructure-as-a-Service, commonly referred to as simply “IaaS,” is a form of cloud
computing that delivers fundamental compute, network, and storage resources to consumers ondemand, over the internet, and on a pay-as-you-go basis. IaaS enables end users to scale and shrink
resources on an as-needed basis, reducing the need for high, up-front capital expenditures or
unnecessary “owned” infrastructure, especially in the case of “spiky” workloads. In contrast to PaaS and
SaaS (even newer computing models like containers and serverless), IaaS provides the lowest-level
control of resources in the cloud. IaaS emerged as a popular computing model in the early 2010s, and
since that time, it has become the standard abstraction model for many types of workloads. However,
with the advent of new technologies, such as containers and serverless, and the related rise of the
microservices application pattern, IaaS remains foundational but is in a more crowded field than ever.
IaaS platform and architecture
 Physical data centers: IaaS providers will manage large data centers, typically around the
world, that contain the physical machines required to power the various layers of abstraction on
top of them and that are made available to end users over the web. In most IaaS models, end
users do not interact directly with the physical infrastructure, but it is provided as a service to
them.
 Compute: IaaS is typically understood as virtualized compute resources, so for the purposes of
this article, we will define IaaS compute as a virtual machine. Providers manage
the hypervisors and end users can then programmatically provision virtual “instances” with
desired amounts of compute and memory (and sometimes storage). Most providers offer both
CPUs and GPUs for different types of workloads. Cloud compute also typically comes paired with
supporting services like auto scaling and load balancing that provide the scale and performance
characteristics that make cloud desirable in the first place.
 Network: Networking in the cloud is a form of Software Defined Networking in which traditional
networking hardware, such as routers and switches, are made available programmatically,
typically through APIs. More advanced networking use cases involve the construction of multizone regions and virtual private clouds, both of which will be discussed in more detail later.
 Storage: The three primary types of cloud storage are block storage, file storage, and object
storage. Block and file storage are common in traditional data centers but can often struggle with
scale, performance and distributed characteristics of cloud. Thus, of the three, object storage has
thus become the most common mode of storage in the cloud given that it is highly distributed
(and thus resilient), it leverages commodity hardware, data can be accessed easily over HTTP,
and scale is not only essentially limitless but performance scales linearly as the cluster grows.
Common IaaS business scenarios
Typical things businesses do with IaaS include:
- Test and development. Teams can quickly set up and dismantle test and development
environments, bringing new applications to market faster. IaaS makes it quick and economical to
scale up dev-test environments up and down.
- Website hosting. Running websites using IaaS can be less expensive than traditional web
hosting.
- Storage, backup, and recovery. Organizations avoid the capital outlay for storage and
complexity of storage management, which typically requires a skilled staff to manage data and
meet legal and compliance requirements. IaaS is useful for handling unpredictable demand and
steadily growing storage needs. It can also simplify planning and management of backup and
recovery systems.
- Web apps. IaaS provides all the infrastructure to support web apps, including storage, web and
application servers, and networking resources. Organizations can quickly deploy web apps on
IaaS and easily scale infrastructure up and down when demand for the apps is unpredictable.
- High-performance computing. High-performance computing (HPC) on supercomputers,
computer grids, or computer clusters helps solve complex problems involving millions of variables
or calculations. Examples include earthquake and protein folding simulations, climate and
weather predictions, financial modeling, and evaluating product designs.
- Big data analysis. Big data is a popular term for massive data sets that contain potentially
valuable patterns, trends, and associations. Mining data sets to locate or tease out these hidden
patterns requires a huge amount of processing power, which IaaS economically provides.
Advantages of IaaS
- Eliminates capital expense and reduces ongoing cost. IaaS sidesteps the upfront expense of
setting up and managing an onsite datacenter, making it an economical option for start-ups and
businesses testing new ideas.
- Improves business continuity and disaster recovery. Achieving high availability, business
continuity, and disaster recovery is expensive, since it requires a significant amount of technology
and staff. But with the right service level agreement (SLA) in place, IaaS can reduce this cost and
access applications and data as usual during a disaster or outage.
- Innovate rapidly. As soon as you’ve decided to launch a new product or initiative, the necessary
computing infrastructure can be ready in minutes or hours, rather than the days or weeks—and
sometimes months—it could take to set up internally.
- Respond quicker to shifting business conditions. IaaS enables you to quickly scale up
resources to accommodate spikes in demand for your application— during the holidays, for
example—then scale resources back down again when activity decreases to save money.
- Focus on your core business. IaaS frees up your team to focus on your organization’s core
business rather than on IT infrastructure.
- Increase stability, reliability, and supportability. With IaaS there’s no need to maintain and
upgrade software and hardware or troubleshoot equipment problems. With the appropriate
agreement in place, the service provider assures that your infrastructure is reliable and meets
SLAs.
- Better security. With the appropriate service agreement, a cloud service provider can provide
security for your applications and data that may be better than what you can attain in-house.
- Gets new apps to users faster. Because you don’t need to first set up the infrastructure before
you can develop and deliver apps, you can get them to users faster with IaaS.

 

 

 

 

 

 

 

 
