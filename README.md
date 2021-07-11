# Managing Cloud-Native Data on Kubernetes - Book Outline

Thanks for looking at the outline and topics for our upcoming book with O'Reilly Media. 
We'd love to get feedback from the community on the topics you'd find useful in a book about data on Kubernetes. 
Please submit an issue or PR on this repo with any suggestions you'd like to make.


## Chapter 1: Introduction to cloud-native data infrastructure: persistence, streaming, and analytics
Takeaway: running databases on Kubernetes has historically been a challenge because it was originally designed for stateless workloads, but this is changing.

*   Current landscape
*   Cloud commodities: compute, networking, storage… and data?
*   The three ingredients of cloud data infrastructure: persistence, streaming, and analytics
*   Overview of desired characteristics: scalability, elasticity, availability, observability, predictable cost
*   Roadmap for the book

## Chapter 2: Managing Stateful Data on Kubernetes
Takeaway: While Kubernetes was originally designed on stateless workloads, it’s extensibility has made it possible to make data a first class citizen

*   Kubernetes primitives for stateful data
    *   Volumes
    *   Persistent volumes
    *   Persistent volume claims
    *   Storage classes
    *   Deployments and replica sets
    *   Stateful sets
*   Kubernetes storage
    *   Container Storage Interface (CSI) 
    *   Container Attached Storage
    *   OpenEBS
    *   Replication: Storage-based vs. database-managed 

## Chapter 3: Running Databases on Kubernetes (the hard way)
Takeaway: running a database yourself on K8s is simple at the scale of a single node, but gets harder as you try to scale up and maintain high availability.

*   Deploying a single-node database
    *   Relational example: MySQL
*   Deploying a distributed database
    *   NoSQL example: Cassandra

## Chapter 4: Automating Database Operations on Kubernetes
Takeaway: The operator pattern provides the critical breakthrough that enables us to simplify database operations in Kubernetes through automation

*   Extending Kubernetes with custom resources
*   The Operator pattern
*   NoSQL Case Study: Cass-operator
*   Relational Case Study: Vitess

## Chapter 5: Streaming Data on Kubernetes
Takeaway: Messaging and streaming technologies are an important complementary technology to databases on Kubernetes for moving data

*   Defining Cloud Native Streaming
*   Case Study: Pulsar
*   Case Study: Flink

## Chapter 6: Integrating Data Infrastructure in a Kubernetes Stack
Takeaway: Databases and data services must provide interfaces for management, monitoring, and security that allow them to be managed as part of an integrated stack. 

*   Data Infrastructure and Site Reliability Engineering
*   High Availability
*   Observability (Metrics, Logging, Tracing)
*   Security (Identity management, Access control, Shared secrets)
*   Cost management (long running resources, data movement)
*   Case study: K8ssandra

## Chapter 7: Data Analytics on Kubernetes
Takeaway: Analytic workloads create an interesting hybrid of stateful and stateless workloads to create an elastic data analysis platform with efficient resource utilization. 

*   Mapping Analytics Workloads to Kubernetes
    *   Stateful and Stateless Workloads
    *   Elastic analytics
*   Building analytics pipelines on Kubernetes
    *   Case study: Apache Spark
    *   Using service mesh to enable secure access for Spark workers
*  Machine Learning and AI
    *   Case study: MLflow

## Chapter 8: Data APIs on Kubernetes
Takeaway: The key to developer productivity on Kubernetes is to stop thinking about database query languages and start coding to data APIs

*   Case studies:companies who have built APIs on top of persistence
*   Required qualities of a data service
*   Data APIs
    *   Case study: Stargate
*   Data as a Service

## Chapter 9: Interacting with Data in Kubernetes Applications
*   Data and Microservice Design Patterns
*   Connecting Microservices to Data
    *   Open Service Broker API
*   Data topologies on K8s
    *   Multi data center
    *   Multi Cloud
    *   Multitenancy
    *   Case study: using a managed service vs. running your own

## Chapter 10: The Cloud Native Database
*   Takeaway: The emerging generation of databases will be based on new architectures in order to truly maximize the benefits of the cloud.
*   Separation of compute and storage
*   Applying Serverless Principles
*   A Maturity Model for Cloud Native Databases
*   Case Study: TBD

## Chapter 11: Emerging Use cases for Data on K8s
Takeaway: In the past, we’ve lived primarily in a world of “app-driven data”. A cloud native approach and technologies will enable us to transition to “data-driven apps”

*   (Each topic below will include a case study)
*   CI/CD
*   Migration to data services
    *   From on prem to cloud
    *   From relational to non relational
*   Analytics
*   AI/ML
    *   Kubeflow - ML model lifecycle
    *   AI Ops
*   Data Mesh 
    *   How cloud native data infrastructure enables data mesh

## Chapter 12: DataOps and Declarative Data
Takeaway: The next great leap forward in data engineering will be the ability to treat data sets as Kubernetes resources and express desired operations and transformations by declaring the desired outcome and allowing your K8s-enabled data stack to do the work.

*   The future state of Data pipelines 
*   Toward a language for declarative data
*   The future of DataOps
*   Case Study: TBD
