
# Møller Digital's Speed Platform: A Journey of Transformation Through Self-Service Cloud Platform

Before 2022, deploying new code changes to customers at Møller Digital was a lengthy process that often took several weeks to complete. 
Development teams faced significant bottlenecks, infrastructure dependencies, and manual processes that hindered innovation and responsiveness. 
Recognizing this critical challenge, Møller Digital made a strategic decision to build a platform centered on self-service capabilities and well-established technologies - 
a solution that would dramatically reduce deployment times while increasing reliability and security.

## Collaborative Beginnings and Technology Foundations

The journey began with developers sitting side by side with the platform team, collaboratively crafting a roadmap for the new platform. 
Rather than reinventing the wheel, we leveraged technologies already established within Møller's ecosystem: Azure provided our cloud foundation, 
Azure DevOps as code repository and code versioning, and Datadog delivered monitoring capabilities.
We also did some choice. For infrastructure as code, we selected Terraform, giving us declarative, version-controlled infrastructure management. Kubernetes (AKS) was chosen as our runtime 
environment, providing container orchestration and scalability. For deployment we chosed ArgoCD. From day one, we made a fundamental commitment: all infrastructure would be set up through code - no manual configurations, no exceptions.

Our first milestone was establishing a functioning runtime environment where applications could be deployed and tested. Progress was methodical and deliberate. Nine months after beginning this journey, 
we celebrated a significant achievement: the first application was running in production on the Speed platform, validating our approach and laying the groundwork for wider adoption.


## From Manual Steps to Seamless Automation

In the early days of the application platform, developers had to perform several manual steps to deploy their applications to the platform. While functional, this approach was still time-consuming 
and prone to human error. However, continuous improvement was built into our platform philosophy.  Throughout 2023, we systematically eliminated these manual processes. We developed reusable Terraform modules 
for the most common Azure resources, dramatically simplifying infrastructure provisioning. The platform evolved to support auto-deployment to test environments, allowing developers to 
see their changes in action without manual intervention.

These automation improvements transformed the developer experience. What once required numerous manual steps and coordination with the platform team could now be accomplished 
through self-service capabilities, letting developers focus on creating value rather than managing deployment logistics. The Speed-platform is born - "Service Platform Enabling Efficient Delivery"

## Agility in Technology Choices

A key principle behind Speed's architecture is the light integration of well-established technologies. This approach has given us remarkable flexibility to swap out components when 
better options emerge, without disrupting the platform's overall functionality. Early in our journey, developers adopted Launch Darkly for feature toggling, allowing them to control
feature releases with precision. However, as our needs evolved, we identified Unleash as a superior alternative—offering better pricing and improved handling of our data. 
The transition was seamless, with no downtime experienced by users.

Similarly, in summer 2023, we migrated from Azure DevOps to GitHub. This significant change in our development toolchain was accomplished without disrupting ongoing projects or 
developer workflows.  These technology transitions have been possible because of two foundational principles: infrastructure as code for all components and minimal customization. 
By maintaining these disciplines, we've created a platform that can evolve alongside technology trends and changing business requirements without costly rebuilds or service interruptions.

## Security by Design
Security has been a cornerstone of the Speed platform from its inception. Rather than treating security as an afterthought or placing the burden entirely on application developers, 
we've built security directly into the platform services, significantly reducing the cognitive load on our development teams.
The platform handles all access management to services and between components within the platform itself. We've implemented complete isolation between environments and between 
different services unless deliberately configured otherwise. This "secure by default" approach ensures that applications can only communicate with other services when explicitly 
permitted, minimizing potential attack surfaces.

In 2024, we began our journey toward implementing Zero Trust principles within the platform. After careful evaluation, we selected Consul as our service mesh solution, 
largely due to its robust connectivity capabilities with our on-premises data center. This choice allows us to maintain consistent security policies across our hybrid infrastructure 
while providing the flexibility needed for our diverse application portfolio.

## Why an Application Platform? Adapting to a Dynamic Market

In today's rapidly evolving market landscape, why is an application platform like Speed essential? We believe the answer lies in the need for organizations to respond 
swiftly to changing conditions and customer expectations. Speed provides a self-service environment where developers can independently implement new changes and adapt to market 
demands without lengthy approval processes or infrastructure provisioning delays. This autonomy is crucial in maintaining competitive advantage when market opportunities emerge or 
shifts occur. Technology itself is changing at an unprecedented pace. The flexibility built into our platform acknowledges this reality, ensuring that Speed can continuously evolve to 
meet the emerging needs of its users. Rather than creating a static solution that will eventually become outdated, we've designed a platform that can transform alongside both business 
requirements and technology advancements. 

This adaptability extends beyond just keeping pace with change—it actively enables it. By providing a stable yet flexible foundation, Speed allows our development teams to focus on 
innovation rather than infrastructure management, creating value for our customers faster than ever before.

