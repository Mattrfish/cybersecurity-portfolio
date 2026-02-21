Terraform is an infrastructure as code tool. It lets you manage infrastructure with config files rather than a GUI, allowing you to build and manage it in a safe, reusable way.



It allows you to define infrastructure in a readable way and can be used on multiple cloud platforms. Its state allows you to track resource changes throughout the deployments. It can be used with version control to safely collab on infrastructure. 



**Managing infrastructure:** Its plugins called providers, let terraform interact with cloud providers using APIs. There are over 1000 providers to manage resources on multiple platfroms like AWS, Azure, GCP, GitHub, Kubernetes etc. 



**Standardise workflow:** Resources, like EC2 instances, can be composed into reusable configs called modules. The config language is declarative and the providers automatically calculate dependencies between resources.



To deploy infrastructure with Terraform:



* Scope - Identify the infrastructure for your project.
* Author - Write the configuration for your infrastructure.
* Initialize - Install the plugins Terraform needs to manage the infrastructure.
* Plan - Preview the changes Terraform will make to match your configuration.
* Apply - Make the planned changes.



**Track infrastructure:** A state file keep track of the infrastructure to determine the changes made to it so that it matches the config.



**Collaborate:** Its remote state backends allow for collaboration on the infrastructure. You can securely share your state with teammates provide a stable environment for terraform to run in and prevent race conditions when multiple people make config changes at once. It can be connected to GitHub for version control.







