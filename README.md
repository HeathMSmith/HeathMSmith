![Banner](./assets/banner.png)

# Hi, I'm Heath

I design production-grade AWS infrastructure using Terraform, with a
focus on private networking, immutable infrastructure, and
cost-optimized architectures.

My work emphasizes real-world patterns including CI/CD pipelines,
NAT-less VPC design, and secure, fully private compute using AWS Systems
Manager.

------------------------------------------------------------------------

Representative projects demonstrating application delivery and
infrastructure design on AWS.

------------------------------------------------------------------------

## Featured Projects

------------------------------------------------------------------------

### Production Web Application (AWS + Terraform)

A production-style application delivery stack focused on exposing a
secure, highly available service to end users.

**Focus Areas:** - Application Load Balancer with HTTPS (ACM + Route
53) - Auto Scaling Group handling dynamic traffic - Private EC2
instances with no public IPs - Secure access via AWS Systems Manager
(SSM, no SSH) - End-to-end request flow from internet to application
layer

**Key Architectural Decision:**\
Eliminated NAT Gateway dependency by leveraging VPC Endpoints and
private DNS, reducing cost while maintaining secure private
connectivity.

**What This Demonstrates:** - Delivering a publicly accessible
application using private compute - Load balancing and traffic
distribution - Secure ingress and TLS termination - Real-world
application access patterns

[View
Example](https://github.com/HeathMSmith/terraform-aws-modules-hms/tree/main/examples/production-webapp)

------------------------------------------------------------------------

### 3-Tier AWS Infrastructure (HA, CI/CD, Immutable Design)

An infrastructure-focused project modeling how production AWS
environments are designed, deployed, and operated.

**Focus Areas:** - Multi-AZ VPC design with 9 subnet segmentation
(public, application, database) - Infrastructure deployment via CI/CD
(GitHub Actions + OIDC) - Immutable compute layer using custom AMIs (no
runtime package installation) - NAT-less architecture using VPC
Interface Endpoints for private connectivity - Full lifecycle management
including controlled apply and destroy workflows

**Key Architectural Decisions:** - Shifted from user_data provisioning
to AMI-based immutable infrastructure for deterministic deployments\
- Eliminated outbound internet dependency from private subnets\
- Designed infrastructure to support safe teardown and redeployment
cycles

**What This Demonstrates:** - Designing secure, segmented network
architectures\
- Building reproducible infrastructure using Terraform modules and
environments\
- Operating infrastructure through CI/CD pipelines\
- Debugging real AWS dependency and lifecycle issues

------------------------------------------------------------------------

## Infrastructure Maturity Signals

-   Remote state management (S3 + DynamoDB locking)\
-   CI/CD pipelines with OIDC authentication (no long-lived
    credentials)\
-   Controlled deployment and teardown workflows\
-   Immutable infrastructure using custom AMIs\
-   Debugged real AWS dependency and teardown issues\
-   Cost optimization through NAT elimination and endpoint usage

------------------------------------------------------------------------

## Core Focus Areas

-   Designing secure, private AWS architectures (no public compute)\
-   Infrastructure as Code with Terraform (modular, multi-environment
    design)\
-   CI/CD for infrastructure (GitHub Actions + OIDC)\
-   Immutable infrastructure patterns (AMI-based deployments)\
-   Cost optimization through architectural decisions

------------------------------------------------------------------------

## Repository Structure

-   modules/ → reusable Terraform modules\
-   examples/ → real-world implementations\
-   environments/ → multi-environment deployments

------------------------------------------------------------------------

## Real-World Debugging Experience

-   Resolved Terraform state lock conflicts using DynamoDB locking
    mechanisms\
-   Diagnosed AWS dependency violations during VPC teardown (ENIs, SGs,
    IGW)\
-   Handled Secrets Manager recovery window conflicts during
    redeployment\
-   Managed drift between Terraform-managed and manually created
    resources

------------------------------------------------------------------------

## Explore the Repository

[View
Repository](https://github.com/HeathMSmith/terraform-aws-modules-hms)

------------------------------------------------------------------------

## Connect

LinkedIn: https://www.linkedin.com/in/heath-m-smith/
