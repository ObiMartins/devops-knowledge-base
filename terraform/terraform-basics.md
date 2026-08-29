# What is Terraform.
Terraform is an open-source tool created by HashiCorp that allows you to define, provision, and manage infrastructure using code. It is a core modern DevOps practices, enabling teams to treat infrastructure with the same way and methodology as software development.

# What Infrastructure as Code (IaC)
Infrastructure as Code is the practice of managing and provisioning computer data centers through machine-readable definition files, rather than physical hardware configuration or interactive configuration tools.

# Several benefits of using IaC:

`Version Control`: Since infrastructure is defined in text files, you can track changes in Git, allowing for rollbacks and audit trails.
`Consistency`: Eliminates "configuration drift" where manual changes cause environments to diverge over time.
`Speed`: You can spin up or tear down complex environments in minutes rather than hours.

# Declarative Configuration
`Terraform uses a declarative model`. This means you describe the desired state of your infrastructure, and Terraform determines the steps required to achieve that state.

`Imperative approach` (Not Terraform): You write a script that tells the computer: "Create a server," then "Wait for it to boot," then "Install Apache," then "Start the service."

`Declarative approach` (Terraform): You write: "I want one web server running with Apache." Terraform reads your code, looks at what is currently running, and automatically calculates the difference (the "delta") to add, change, or remove resources to match your code

# Core Concepts
`.tf files`: These are the text files where you write your infrastructure configuration using HCL (HashiCorp Configuration Language). They are human-readable and define your architecture.

`Providers`: These are plugins that allow Terraform to communicate with various cloud platforms or services (e.g., AWS, Azure, Google Cloud, GitHub, Kubernetes). Without a provider, Terraform would not know how to "talk" to the target platform.

`Resources`: These are the individual components you are managing (e.g., a specific virtual machine, a database instance, a network subnet, or a firewall rule).

`Modules`: A module is a container for multiple resources that are used together. Think of them as "functions" in programming; you can write a module for a "standard web server stack" and reuse that module across different projects.


# How Terraform Works
The "magic" of Terraform lies in its State File (terraform.tfstate).

When you create infrastructure, Terraform records the IDs and details of those resources in a JSON file called the state file. When you run Terraform again, it performs the following:

`Refresh`: It reads the state file and queries the actual provider (e.g., AWS) to see what is currently out in the real world.

`Plan`: It compares your code (desired state) against the state file and the real-world infrastructure. It calculates the necessary actions to reach your desired state.

`Apply`: It executes those actions (API calls) to update the infrastructure.


# The Terraform Workflow
The standard workflow for managing infrastructure follows a simple cycle:

`Write`: Create or update your .tf files.

`Plan`: Run terraform plan to see what changes Terraform intends to make. This is a critical safety step.

`Apply`: Run terraform apply to execute the planned changes and modify your infrastructure.