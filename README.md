# Managing Cloud-Native Data on Kubernetes - Book Outline

Thanks for looking at the outline and topics for our upcoming book with O'Reilly Media. 
We'd love to get feedback from the community on the topics you'd find useful in a book about data on Kubernetes. 
Please submit an issue or PR on this repo with any suggestions you'd like to make.


## Chapter 1: Introduction to cloud-native data infrastructure: persistence, streaming, and analytics
Takeaway: we've come a long way in defining what cloud-native means for stateless applications, but it's time to establish a vision for cloud-native data infrastructure and stateful applicaitons that can help us leverage the power of Kubernetes for the next generation of technology.

*   Stateless vs. stateful services
*   What is Cloud Native Data?
*   Cloud commodities: compute, networking, storage… and data?
*   The three ingredients of cloud data infrastructure: persistence, streaming, and analytics
*   Overview of desired characteristics: scalability, elasticity, availability, observability, predictable cost

## Chapter 2: Managing Data Storage on Kubernetes
Takeaway: Kubernetes provides the storage primitives that establish a foundation for building cloud-native stateful applications.

*   Background: Container Storage in Docker
*   Kubernetes primitives for data storage
    *   Volumes
    *   Persistent volumes
    *   Persistent volume claims
    *   Storage classes
*   Kubernetes storage extensions
    *   Container Storage Interface (CSI) 
    *   Container Attached Storage (i.e. OpenEBS)
    *   Container Object Storage Interface (COSI)

## Chapter 3: Running Databases on Kubernetes (the hard way)
Takeaway: running a database yourself on K8s is simple at the scale of a single node, but gets harder as you try to scale up and maintain high availability.

*  Kubernetes primitives for managing stateful workloads
    *   Deployments and replica sets
    *   Stateful sets
*   Deploying a single-node database
    *   Relational example: MySQL
*   Deploying a distributed database
    *   NoSQL example: Cassandra

## Chapter 4: Automating Database Deployment on Kubernetes with Helm
Takeaway: Deployments of stateful applications on K8s can get complicated pretty quickly. We need tools like Helm to help automate the deployment and update of K8s resources.

*   Helm and other package managers
*   Using Helm to deploy MySQL
    *   Additional K8s resources: Secrets, ConfigMaps, ServiceAccounts
*   Using Helm to deploy Apache Cassandra
    *   Affinity and anti-affinity
*   Limitations of Helm for application operations

## Chapter 5: Automating Database Management on Kubernetes with Operators
Takeaway: The operator pattern provides the critical breakthrough that enables us to simplify database operations in Kubernetes through automation

*   Extending Kubernetes with custom resources
*   The Operator pattern
*   NoSQL Case Study: Cass-operator & Medusa
*   Relational Case Study: Vitess

## Chapter 6: Integrating Data Infrastructure in a Kubernetes Stack
Takeaway: Databases and data services must provide interfaces for management, monitoring, and security that allow them to be managed as part of an integrated stack. 

*   Considerations in developing integrated stacks
    *   High Availability
    *   Observability (Metrics, Logging, Tracing)
    *   Security (Identity management, Access control, Shared secrets)
    *   Cost management (long running resources, data movement)
*   Case study: K8ssandra
    *   Deployment
    *   Monitoring 
    *   Maintenance
    *   Multi-cluster/multi-datacenter operations
*   The Data Gateway pattern - Data as a Service
    *   Case study: Stargate

## Chapter 7: The Kubernetes Native Database
*   Takeaway: The emerging generation of databases will be based on new architectures in order to truly maximize the benefits of the cloud.
*   Why a Kubernetes Native Approach is Needed
*   Hybrid data access at scale with TiDB
*   Serverless Cassandra with DataStax AstraDB
*   What to look for in a Kubernetes Native Database
   
## Chapter 8: Streaming Data on Kubernetes
Takeaway: Messaging and streaming technologies are an important complementary technology to databases on Kubernetes for moving data

*   Defining Cloud Native Streaming
*   Case Study: Pulsar
*   Using service discovery in streaming
*   Case Study: Flink

## Chapter 9: Data Analytics on Kubernetes
Takeaway: Analytic workloads create an interesting hybrid of stateful and stateless workloads to create an elastic data analysis platform with efficient resource utilization. 

*   Mapping Analytics Workloads to Kubernetes
    *   Stateful and Stateless Workloads
    *   Elastic analytics
*   Building analytics pipelines on Kubernetes
    *   Case study: Apache Spark
    *   Using service mesh to enable secure access for Spark workers

## Chapter 10: Emerging Use cases for Data on K8s
Takeaway: In the past, we’ve lived primarily in a world of “app-driven data”. A cloud native approach and technologies will enable us to transition to “data-driven apps”

*   (Each topic below will include a case study)
*   CI/CD
*   Migration to data services
    *   From on prem to cloud
    *   From relational to non relational
    *   implications for data pipelines
*   Analytics
*   AI/ML
    *   Kubeflow - ML model lifecycle
    *   AI Ops
*   Data Mesh 
    *   How cloud native data infrastructure enables data mesh
*   Declarative data
    *   Treat data sets as Kubernetes resources and express desired operations and transformations by declaring the desired state

## Chapter 11: Migrating Data Workloads to Kubernetes
Takeaway: Let's make a plan to take advantage of everything you've learned in the book.

*   The vision: Application-Aware Platforms
*   Sidebar with Craig McLuckie
*   Charting your Path to Success
    *   People - roles and communities
    *   Technology - selection criteria, architecture approaches
    *   Process - prerequisites, migration recommendations
*   Sidebar - a vision of a cloud native data future

