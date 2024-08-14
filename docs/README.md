<!-- TODO: Update with your values. -->
<!-- # Beamstack -->

<div align="center">
    <picture>
        <img src="https://raw.githubusercontent.com/BeamStackProj/webpage/master/docs/logo.png" alt="logo" width="600">
    </picture>
</div>

 <!-- TODO: Update repo links and change license type if needed. -->


<!-- TODO: You can delete the About and Create a Docsify site sections if you create a new project from this template -->

## Overview

### What is Beamstack?
Beamstack is a command line interface (CLI) tool that makes deploying machine learning workflows easier with Apache Beam on Kubernetes. 

Beamstack is a revolutionary tool that has been meticulously crafted to simplify and revolutionize the deployment of machine learning (ML) workflows on Kubernetes. It offers a holistic solution by introducing abstraction layers that streamline the deployment of diverse components of ML pipelines, data processing workflows, and deployment infrastructure.

At the heart of Beamstack's capabilities lie Kubernetes Custom Resource Definitions (CRDs). These CRDs serve as a powerful mechanism for extending the Kubernetes API, enabling the seamless integration of ML-specific resources into the Kubernetes ecosystem. Through this innovative approach, Beamstack empowers users to leverage the robust features and functionalities of Kubernetes while unlocking the immense potential of ML.

With Beamstack, deploying and managing complex ML workflows becomes an effortless endeavor. It provides a unified interface that allows users to define, configure, and monitor their ML pipelines in a declarative manner. By abstracting away the underlying complexities of Kubernetes, Beamstack empowers data scientists, engineers, and DevOps professionals to focus on their core competencies and deliver impactful ML solutions.

Moreover, Beamstack offers a rich set of features that enhance the efficiency and scalability of ML deployments. It includes built-in support for popular ML frameworks, such as TensorFlow, PyTorch, and Apache MXNet, enabling users to seamlessly integrate their existing ML models into Kubernetes environments. Additionally, Beamstack provides automated resource provisioning, ensuring that ML components have the necessary resources to perform optimally.

Beamstack is designed to be flexible and extensible, allowing users to customize their deployments based on their specific requirements. It supports various deployment options, including on-premises, cloud, and hybrid environments, providing the freedom to choose the infrastructure that best suits their needs.

### Why Beamstack?
Deploying machine learning and GenAI workflows should be easy. By extension, managing those workflows should be easy as well, beamstack offers a solution that streamlines the deployment process of complex workflows. It is an open-source tool, easy to understand, and versatile. 

### Architecture
----

<div>
    <picture>
        <source srcset="https://raw.githubusercontent.com/BeamStackProj/webpage/master/docs/arch-dark.png" media="(prefers-color-scheme:dark)">
        <img src="https://raw.githubusercontent.com/BeamStackProj/webpage/master/docs/architecture-light.png" media="(prefers-color-scheme:light)"alt="Architecture Diagram" width="1000">
    </picture>
</div>

### How it works
----
Beamstack has a simple and intuitive flow of operation explained below.

1. **User Interaction**: The process begins with the user, who interacts with Beamstack using the Beam YAML file. This YAML file defines the machine learning (ML) workflows, data processing tasks, and deployment configurations.

2. **Beam YAML File**: This file contains the specifications for the ML pipeline, such as the type of data processing required, the models to be used, and how they should be deployed on Kubernetes.

3. **Beamstack**: Beamstack takes the YAML configuration and processes it. It converts the YAML specifications into a set of Kubernetes Custom Resource Definitions (CRDs) and deployment configurations that Kubernetes can understand. This ultimately abstracts the complexities of Kubernetes and simplifies the deployment process. 

4. **Kubernetes Integration**: Beamstack integrates with various Kubernetes operators for different runners like Apache Spark, Apache Samza, etc. These operators are responsible for executing the distributed data processing tasks defined in the Beam YAML file.

5. **Worker Pool**: Within the Kubernetes cluster, a pool of workers (Beamstack Harness instances) is deployed. These workers are responsible for running the ML workflows and data processing tasks as defined by the user. Each instance of Beamstack Harness runs a part of the pipeline, ensuring that the workload is distributed efficiently across the cluster.

6. **Data Storage**: The data processed by the workflows is stored in a centralized data storage system, which is also part of the Kubernetes ecosystem. Beamstack ensures that data is stored and retrieved efficiently during the pipeline execution.

7. **Monitoring Stack**: Beamstack includes a monitoring stack that leverages Grafana and Prometheus. This stack continuously monitors the health and performance of the ML workflows and the underlying infrastructure. It provides insights into resource utilization, pipeline performance, and any potential issues.

8. **Multi-Environment Support**: Beamstack is designed to be flexible and can be deployed in various environments, including on-premises data centers, cloud platforms like AWS, Azure, and Google Cloud, or a hybrid setup. This flexibility allows users to choose the infrastructure that best fits their needs.

----

### Features
- Robust Command Line Tool
- Simple Abstraction Layers
- CRD-Based Deployments
- Cross-platform Compatibility
- Configuration Management
- Customization Options
- Monitoring and Visualization
- Integration with data and communication tools
- Unified pipeline for all data
- All-Inclusive Support
- Versioning & Updates


### Development Status
Beamstack is being actively developed. Our releases can be found [here](https://github.com/BeamStackProj/beamstack-cli)

## Understand the Basics

### Learn the Fundamentals
!> Internalize Docker and Kubernetes tutorials
- [A Beginner-Friendly Introduction to Containers, VMs and Docker](https://www.freecodecamp.org/news/a-beginner-friendly-introduction-to-containers-vms-and-docker-79a9e3e119b)
- [Introduction to Kubernetes](https://www.edx.org/learn/kubernetes/the-linux-foundation-introduction-to-kubernetes)
- [More Kubernetes Tutorials](https://kubernetes.io/docs/tutorials/)



## Core Concepts
?> Assuming you are familiar with Docker, Kubernetes, and Machine Learning, Below are some concepts that separate Beamstack from other tools such as kubectl.

### Robust CLI tool
Beamstack comes equipped with a robust Command-Line Interface (CLI) tool, providing users with a powerful method to install, deploy, and manage resources within the Beamstack ecosystem. With this CLI tool, users can seamlessly interact with the resources managed by Beamstack, enabling efficient configuration, monitoring, and updating of machine learning workflows.

### Abstraction Layers
Beamstack introduces intuitive abstraction layers that allow users to define and deploy ML pipeline components with ease. This abstraction simplifies the intricate details of Kubernetes manifests, making deployment accessible to both beginners and experienced users.

### CRD-based Deployments
Leveraging the power of Kubernetes Custom Resource Definitions, Beamstack enables users to express their deployment specifications in a declarative manner. This approach not only enhances readability but also facilitates the effortless scaling and management of resources.

### Infrastructure Agnosticism
Beamstack empowers users to create data pipelines that are agnostic to the underlying infrastructure. Whether you're running on a small computer, in the cloud, or on-premises, Beamstack seamlessly adapts to your environment, ensuring consistent performance and reliability across diverse deployment scenarios.

### Monitoring and Visualization
Beamstack provides comprehensive monitoring capabilities, allowing users to visualize the state of containers and resources within their pipelines. With intuitive dashboards and real-time insights, users can effortlessly track the health and performance of their deployments, facilitating proactive management and optimization.

### Integration with Data Stores and Message Queues
Serving as a conduit for data production, Beamstack enables seamless integration with vector stores, feature stores, and message queues. Whether you're storing feature vectors, persisting data for analysis, or facilitating communication between components, Beamstack streamlines the data flow process, ensuring efficient data handling and interoperability across the pipeline.

### Unified Pipeline for Streaming and Batch Data
Beamstack offers a unified pipeline architecture that caters to both streaming data and batch datasets. Whether you're processing real-time streams or large-scale batch data, Beamstack provides the necessary abstractions and components to orchestrate end-to-end workflows, simplifying the development and deployment of hybrid data processing solutions.

## Getting Started

?> This guide assumes you have a grounded understanding in the tools that Beamstack is based on. Please read [understanding the basics]() to learn about these tools.

### Requirements
!> [Kubectl](https://kubernetes.io/docs/tasks/tools/) must be installed on your local machine

### Install Beamstack CLI
?> Download and run the latest Beamstack version from [here](https://github.com/BeamStackProj/beamstack-cli/tree/main/releases).

?>Run `Beamstack version` to verify that it has been successfully installed

## Usage

### Use Cases

- **ML Pipeline Components**: Define and deploy individual components of your machine learning pipeline, such as data preprocessors, model trainers, and result evaluators, using intuitive CRDs.

- **Data Processing Pipelines**: Seamlessly orchestrate data processing workflows, managing tasks like data ingestion, transformation, and storage with the flexibility provided by Beamstack.

- **Deployment Infrastructure**: Efficiently provision and manage deployment infrastructure resources, ensuring that your machine learning models run optimally in a Kubernetes environment.

### Basic Examples

#### Initialize a Kubernetes Cluster with Beamstack & Monitoring tools
> `beamstack init -m`

#### Get the current kubernetes cluster context and profile info
> `beamstack info`

#### Display the name, status and age of a cluster
> `beamstack info cluster`

#### Create a flink cluster
> `beamstack create flink-cluster [cluster-name]`

#### Open up flink UI
> `beamstack open flink [flink-cluster-name]`

#### Open up Grafana dashboard
> `beamstack open dashboard`


## CLI Command Reference

### beamstack init
**Description:** Initialize Beamstack in a new Kubernetes environment, setting up essential configurations and prerequisites.  
**Arguments:**  
- `--config`: Specify a custom path to a configuration file.
- `--provider`: Specify the cloud or on-premise provider for the cluster.

### beamstack install
**Description:** Install Beamstack components or complete setups necessary to get Beamstack operational within the Kubernetes cluster.  
**Subcommands:**  
- `component`: Install a specific Beamstack component.
- `all`: Install all necessary Beamstack components.

**Arguments for component:**  
- `--name`: Name of the component to install.

**Flags:**  
- `--version`: Specify the version of the component.
- `--dry-run`: Simulate installation without making changes.

### beamstack update
**Description:** Update Beamstack components or configurations to newer versions or to alter existing setups.  
**Subcommands:**  
- `component`: Update a specific Beamstack component.
- `config`: Update Beamstack configuration settings.

**Arguments for component:**  
- `--name`: Name of the component to update.

**Flags:**  
- `--version`: Specify the version of the component.
- `--force`: Force the update, ignoring conflicts.
- `--namespace`: Specify the namespace.

### beamstack version
**Description:** This command returns the current version of Beamstack installed on the host device.

### beamstack deploy
**Description:** Deploy resources or applications managed by Beamstack into the Kubernetes cluster, applying configurations defined by the user.  
**Subcommands:**  
- `workflow`: Deploy a machine learning workflow.

**Arguments for workflow:**  
- `--file`: Path to the workflow configuration file.

**Flags:**  
- `--namespace`: Specify the namespace.
- `--environment`: Specify the deployment environment.
- `--rollback`: Enable rollback on failure.

### beamstack delete
**Description:** Remove Beamstack components, workflows, or other resources from the Kubernetes environment, cleaning up all associated configurations.  
**Subcommands:**  
- `component`: Remove a specific Beamstack component.
- `workflow`: Remove a deployed workflow.

**Arguments for workflow:**  
- `--name`: Name of the workflow to remove.

**Flags:**  
- `--namespace`: Specify the namespace.
- `--force`: Force deletion, ignoring dependencies.

### beamstack status
**Description:** Check the current status of various Beamstack resources, including components and workflows, providing a snapshot of their operational state.  
**Subcommands:**  
- `workflow`: Check the status of a deployed workflow.

**Arguments for workflow:**  
- `--name`: Name of the workflow to check.

**Flags:**  
- `--namespace`: Specify the namespace.

### beamstack config
**Description:** Manage configuration settings for Beamstack, allowing customization and parameter adjustments for different operational environments.  
**Subcommands:**  
- `set`: Set a configuration parameter.
- `get`: Get the value of a configuration parameter.

**Arguments for set and get:**  
- `--key`: Configuration key.
- `--value` (for set): Value to set.

### beamstack help
**Description:** Provide help and documentation for using the Beamstack CLI, explaining commands and their purposes.  
**Arguments for:**  
- `command`: Command to get help on.

### beamstack fetch
**Description:** Retrieve information from the backend.  
**Flags:**  
- `--namespace`: Specify the namespace.


<!-- ## FAQs

- Placeholder 1
- Placeholder 2
- Placeholder 3
- Placeholder 4
- Placeholder 5 -->


## Support

- Make sure you've read understanding the basics and the getting started guide.
- Looked for an answer in the frequently asked questions.
- Read existing [issues](https://github.com/BeamStackProj/beamstack-cli/issues)
- Ask a question in the Beamstack [discord channel](https://discord.gg/fYNnNVaEFK)
- Report a bug, or request a feature

## Become a contributor
- Join our discord channel [here](https://discord.gg/fYNnNVaEFK)


## Roadmap

The Beamstack Roadmap is maintained in a [GitHub Project]()

## Releases

You can find our releases [here]()
