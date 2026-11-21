# Cloud Service Selection Chart

| Example | Service Model | Deployment Model | Reason |
|---|---|---|---|
| Renting a virtual server to host a web app | IaaS | Public | You get a virtual machine (such as an EC2 instance) and manage the OS and software yourself. A public cloud provides this without buying hardware. |
| Managed app hosting for a student project | PaaS | Public | You deploy code while the provider handles servers, OS patches, and scaling. This suits developers who want to focus on the app. |
| Gmail or Google Docs for a college | SaaS | Public | The provider runs the whole application. Users only log in and use it, with no servers or software to manage. |
| A bank's customer database kept in its own data center | IaaS | Private | Regulations and security needs may require the data to stay on infrastructure the bank controls. |
| An e-commerce site that uses cloud servers for peak sales but keeps payment records on-premises | IaaS | Hybrid | The site scales in the public cloud during busy periods, while sensitive data stays in a private environment. |

## Shared Responsibility Model

AWS is responsible for security *of* the cloud. This includes the physical data centers, hardware, networking, and the virtualization layer that runs EC2 instances.

I am responsible for security *in* the cloud. This includes my data, IAM users and permissions, security group rules, OS patches on my EC2 instances, and S3 bucket policies.
