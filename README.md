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

I HAVE PROVIDED IN‑DEPTH EXPLANATIONS FOR EACH QUESTION, AIMED AT ENHANCING YOUR CONCEPTUAL UNDERSTANDING AND PRACTICAL KNOWLEDGE. ADDITIONALLY, I HAVE INCLUDED THE OFFICIAL TERRAFORM DOCUMENTATION LINKS FOR EACH TOPIC COVERED IN THE QUESTIONS AND DISCUSSIONS, ENSURING YOU CAN EXPLORE FURTHER AND VALIDATE EVERY CONCEPT. I HOPE THESE RESOURCES PROVE VALUABLE AND HELP YOU STRENGTHEN YOUR EXPERTISE, THANKYOU!!

`1`. What are some of the features of `Terraform state`?

Ans --

- `mapping configuration to real-world resources`
 Explanation--
`Terraform state` maps configuration to real-world resources by storing the mapping between the desired infrastructure configuration defined in Terraform files and the actual resources created in the cloud environment. This mapping helps Terraform to manage and update resources accurately.   

-`increased performance`
Explanation--
`Terraform state` provides increased performance by storing the current state of managed infrastructure resources. This allows Terraform to efficiently track changes and manage resources without having to query the cloud provider's API repeatedly.

-`determining the correct order to destroy resources`
Explanation--
`Terraform state` helps in determining the correct order to destroy resources by keeping track of dependencies between resources. This ensures that resources are destroyed in the correct sequence to avoid any issues or errors during the destruction process.

Overall explanation--
`Terraform state` provides increased performance by storing the current state of managed infrastructure resources. This allows Terraform to efficiently track changes and manage resources without having to query the cloud provider's API repeatedly.
Terraform state helps in determining the correct order to destroy resources by keeping track of dependencies between resources. This ensures that resources are destroyed in the correct sequence to avoid any issues or errors during the destruction process.

See this [page]https://developer.hashicorp.com/terraform/language/state/purpose on the purpose of Terraform state and the benefits it provides