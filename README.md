THESE NOTES FOCUSES ON THESE OBJECTIVES--

Objective 1 - Understand Infrastructure as Code Concepts    
Objective 2 - Understand Terraform's Purpose (vs other IaC)    
Objective 3 - Understand Terraform Basics    
Objective 4 - Use Terraform Outside of Core Workflow    
Objective 5 - Interact with Terraform Modules  
Objective 6 - Use the core Terraform workflow  
Objective 7 - Implement and Maintain State  
Objective 8 - Read, Generate, and Modify Configuration  
  
Tips to get the most out of it --  
✅ Hands‑on practice is key. Don’t just read — run Terraform locally:  
Create and destroy resources on a free cloud (AWS free tier works).  
Experiment with remote state in S3 or Terraform Cloud.  
✅ Understand, don’t memorize.  
Why use modules? Why use workspaces? What problem does state solve?  
✅ Use the HashiCorp official study guide:  
✅ Do practice questions.  
Tutorials Dojo, Udemy, or free GitHub question banks.  
  
I HAVE PROVIDED IN‑DEPTH EXPLANATIONS FOR EACH QUESTION, AIMED AT ENHANCING YOUR CONCEPTUAL UNDERSTANDING AND   PRACTICAL KNOWLEDGE. ADDITIONALLY, I HAVE INCLUDED THE OFFICIAL TERRAFORM DOCUMENTATION LINKS FOR EACH TOPIC   COVERED IN THE QUESTIONS AND DISCUSSIONS, ENSURING YOU CAN EXPLORE FURTHER AND VALIDATE EVERY CONCEPT. I HOPE THESE   RESOURCES PROVE VALUABLE AND HELP YOU STRENGTHEN YOUR EXPERTISE, THANKYOU!!  
  
`1`. What are some of the features of `Terraform state`?  
  
Ans --  
  
- `mapping configuration to real-world resources`  
 Explanation--  
`Terraform state` maps configuration to real-world resources by storing the mapping between the desired infrastructure configuration defined in Terraform files and the actual resources created in the cloud environment. This mapping helps Terraform to manage and update resources accurately.     
  
- `increased performance`  
Explanation--  
`Terraform state` provides increased performance by storing the current state of managed infrastructure resources. This allows Terraform to efficiently track changes and manage resources without having to query the cloud provider's API repeatedly.  
  
- `determining the correct order to destroy resources`  
Explanation--  
`Terraform state` helps in determining the correct order to destroy resources by keeping track of dependencies between resources. This ensures that resources are destroyed in the correct sequence to avoid any issues or errors during the destruction process.  
  
Overall explanation--  
`Terraform state` provides increased performance by storing the current state of managed infrastructure resources. This allows Terraform to efficiently track changes and manage resources without having to query the cloud   provider's API repeatedly.
Terraform state helps in determining the correct order to destroy resources by keeping track of dependencies between resources. This ensures that resources are destroyed in the correct sequence to avoid any issues or errors during the destruction process.  
  
See this https://developer.hashicorp.com/terraform/language/state/purpose on the purpose of Terraform state and the benefits it provides  

`2` What advantages does Terraform offer over using a provider's native tooling for deploying resources in multi-cloud environments? (Any three)

Ans-- 
- Terraform simplifies management and orchestration, helping operators build large-scale, multi-cloud infrastructure
- Terraform can manage cross-cloud dependencies
- Terraform can help businesses deploy applications on multiple clouds and on-premises infrastructure

Overall Explanation-  
Terraform offers several advantages over using a provider's native tooling for deploying resources in multi-cloud environments, including:

`Multi-cloud support`: Terraform provides a consistent interface for managing infrastructure resources across multiple cloud providers, including AWS, Azure, Google Cloud, and more. This allows organizations to use a single tool for managing their entire multi-cloud environment rather than needing to learn and use multiple provider-specific tools.

`Standardized configuration`: Terraform uses a declarative configuration language to define infrastructure resources, which can be used to define resources across multiple providers in a standardized way. This provides consistency and reduces the need for provider-specific knowledge.

`Idempotent execution`: Terraform only makes changes to infrastructure resources if the desired state differs from the current state, which means that it can be safely run multiple times without causing unintended changes. This reduces the risk of configuration drift and ensures that infrastructure remains consistent over time.

`Plan preview`: Terraform can generate a plan that shows the changes it will make to infrastructure resources before it applies them. This provides visibility into changes and helps to reduce the risk of unintended consequences.

`Collaboration and version control`: Terraform configurations can be stored in version control systems, allowing multiple team members to collaborate on infrastructure changes. This provides a centralized location for documentation, change history, and issue tracking, making it easier to manage infrastructure changes over time.

Overall, using Terraform for deploying resources in multi-cloud environments can provide a consistent, standardized, and efficient approach to managing infrastructure across multiple providers.

https://developer.hashicorp.com/terraform/intro/use-cases#multi-cloud-deployment