# Kubernetes
Just as containers are a portable way of defining software, Kubernetes resources provide a portable definition of how that software should run.
# GCP autopilot 
In 2021, Google Cloud Platform (GCP) released a new offering to their existing Kubernetes service called Autopilot that handles cluster upgrades, networking, and scaling the VMs up and down depending on the demand.
Other cloud providers are also moving in that direction and offering Kubernetes-based platforms where developers only need to worry about running their application and not focus on the underlying infrastructure.

# So let’s look at a few of the characteristics of cloud native systems that most people can agree on:

**Automatable**

If applications are to be deployed and managed by machines, instead of humans, they need to abide by common standards, formats, and interfaces. Kubernetes provides these standard interfaces in a way that means application developers don’t even need to worry about them.

**Ubiquitous and flexible**

Because they are decoupled from physical resources such as disks, or any specific knowledge about the compute node they happen to be running on, containerized microservices can easily be moved from one node to another, or even one cluster to another.

**Resilient and scalable**

Traditional applications tend to have single points of failure: the application stops working if its main process crashes, or if the underlying machine has a hardware failure, or if a network resource becomes congested. Cloud native applications, because they are inherently distributed, can be made highly available through redundancy and graceful degradation.

**Dynamic**

A container orchestrator such as Kubernetes can schedule containers to take maximum advantage of available resources. It can run many copies of containers to achieve high availability, and perform rolling updates to smoothly upgrade services without ever dropping traffic.

**Observable**

Cloud native apps, by their nature, are harder to inspect and debug. So a key requirement of distributed systems is observability: monitoring, logging, tracing, and metrics all help engineers understand what their systems are doing (and what they’re doing wrong).

**Distributed**

Cloud native is an approach to building and running applications that takes advantage of the distributed and decentralized nature of the cloud. It’s about how your application works, not where it runs. Instead of deploying your code as a single entity (known as a monolith), cloud native applications tend to be composed of multiple, cooperating, distributed microservices. A microservice is simply a self-contained service that does one thing. If you put enough microservices together, you get an application.

**SRE**

At this point, not every developer can be an infrastructure expert, just as a single team of infrastructure experts can’t service an ever-growing number of developers. For larger organizations, while a central infrastructure team is still needed, there’s also a case for embedding site reliability engineers (SREs) into each development or product team. They bring their expertise to each team as consultants and also form a bridge between product development and infrastructure operations.

**Docker**
Containers allow you to deploy and run software in small, standardized, self-contained units. This makes it easier and cheaper to build large, diverse, distributed systems, by connecting together containerized microservices.

**Kubernetes**
Orchestration systems take care of deploying your containers, scheduling, scaling, networking, and all the things that a good system administrator would do, but in an automated, programmable way.
