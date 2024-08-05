<!-- TODO: Update with your values. -->
# Beamstack
> CLI Tool for Deploying ML Workflows

 <!-- TODO: Update repo links and change license type if needed. -->

[![Made with latest Docsify](https://img.shields.io/npm/v/docsify/latest?label=docsify)](https://docsify.js.org/)


<!-- TODO: You can delete the About and Create a Docsify site sections if you create a new project from this template -->

## Overview

### What is Beamstack?
Beamstack is a command line interface (CLI) tool that makes deploying machine learning workflows easier with Apache Beam on Kubernetes. 

Beamstack is a revolutionary tool that has been meticulously crafted to simplify and revolutionize the deployment of machine learning (ML) workflows on Kubernetes. It offers a holistic solution by introducing abstraction layers that streamline the deployment of diverse components of ML pipelines, data processing workflows, and deployment infrastructure.

At the heart of Beamstack's capabilities lie Kubernetes Custom Resource Definitions (CRDs). These CRDs serve as a powerful mechanism for extending the Kubernetes API, enabling the seamless integration of ML-specific resources into the Kubernetes ecosystem. Through this innovative approach, Beamstack empowers users to leverage the robust features and functionalities of Kubernetes while unlocking the immense potential of ML.

With Beamstack, deploying and managing complex ML workflows becomes an effortless endeavor. It provides a unified interface that allows users to define, configure, and monitor their ML pipelines in a declarative manner. By abstracting away the underlying complexities of Kubernetes, Beamstack empowers data scientists, engineers, and DevOps professionals to focus on their core competencies and deliver impactful ML solutions.

Moreover, Beamstack offers a rich set of features that enhance the efficiency and scalability of ML deployments. It includes built-in support for popular ML frameworks, such as TensorFlow, PyTorch, and Apache MXNet, enabling users to seamlessly integrate their existing ML models into Kubernetes environments. Additionally, Beamstack provides automated resource provisioning, ensuring that ML components have the necessary resources to perform optimally.

Beamstack is designed to be flexible and extensible, allowing users to customize their deployments based on their specific requirements. It supports various deployment options, including on-premises, cloud, and hybrid environments, providing the freedom to choose the infrastructure that best suits their needs.


<!-- <div align="center">
    <a href="https://michaelcurrin.github.io/docsify-js-tutorial/">
        <img src="https://img.shields.io/badge/Teach_me-DocsifyJS_tutorial-blue" 
            alt="DocsifyJS tutorial badge"
            title="Go to tutorial">
    </a>
</div> -->

### Why Beamstack?
Deploying machine learning and GenAI workflows should be easy. By extension, managing those workflows should be easy as well, beamstack offers a solution that streamlines the deployment process of complex workflows. It is an open-source tool, easy to understand, and versatile. 

### How it works
Imagine you have a big box of Lego bricks and want to build a cool spaceship. But instead of figuring out which bricks to use and where to put them, you have a magical helper called Beamstack that does it all for you!

Here's how Beamstack works, step by step as if you're playing with Legos:

- **Easy Commands**: Beamstack allows you to enter simple commands, like a Lego manual, to build different parts of your spaceship (which is your machine learning project).


- **Special Blocks (CRDs)**: Beamstack has special Lego blocks called CRDs (Custom Resource Definitions). These blocks are super smart and know exactly how to fit into your spaceship to make it work perfectly.


- **Tell Beamstack What You Want**: You tell Beamstack what kind of spaceship you want by giving it a list of parts (like engines, wings, and control panels). This list is like a recipe for your spaceship. This can be done by providing a YAML file with the appropriate components you wish for. 


- **Beamstack Builds for You**: Beamstack takes your list and starts building. It uses the special blocks (CRDs) and puts them together in the right way, just like following a Lego manual.


- **Magic Assembly Line**: Beamstack has a magic assembly line that works super fast. It puts all the parts together and checks to make sure everything is perfect.


- **Watch Your Spaceship Fly**: Once Beamstack is done, your spaceship is ready to fly! You can see it in action, zooming around and doing all the cool things you wanted it to do.


- **Keep an Eye on It**: Beamstack also helps you keep an eye on your spaceship. It has a special control panel where you can see how your spaceship is doing, if it needs more fuel, or if any parts need fixing.


- **Works Everywhere**: The best part is, Beamstack can build spaceships anywhere! Whether you want it to work in your backyard (local computer), at a friend's house (on-premises), or in the clouds (cloud services), Beamstack can do it all.

### Architecture
<img src="https://github.com/BeamStackProj/webpage/blob/master/docs/arch.png">

### Features
- Robust Command Line Tool
- Simple Abstraction Layers
- CRD-Based Deployments
- Cross-platform Compatibility
- Monitoring and Visualization
- Integration with data and communication tools
- Unified pipeline for all data
- All-Inclusive Support


### Development Status
Beamstack is being actively developed. Our releases can be found here

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
> - Download and run the latest Beamstack version from [here](https://github.com/BeamStackProj/beamstack-cli/tree/main/releases).

> - Run `Beamstack version` to verify that it has been successfully installed

## Usage

### Use Cases

- **ML Pipeline Components**: Define and deploy individual components of your machine learning pipeline, such as data preprocessors, model trainers, and result evaluators, using intuitive CRDs.

- **Data Processing Pipelines**: Seamlessly orchestrate data processing workflows, managing tasks like data ingestion, transformation, and storage with the flexibility provided by Beamstack.

- **Deployment Infrastructure**: Efficiently provision and manage deployment infrastructure resources, ensuring that your machine learning models run optimally in a Kubernetes environment.

### Basic Examples

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
- Read existing issues
- Ask a question in the Beamstack Slack channel 
- Report a bug, or request a feature

## Roadmap

The Beamstack Roadmap is maintained in a [GitHub Project]()

## Releases

You can find our releases [here]()
