# Beginner Docker Guide

## 1. Virtualization

**Virtualization** allows multiple virtual machines (VMs) to run on a single physical machine, managed by a hypervisor.

- **Type 1 Hypervisor**: Runs on hardware (e.g., VMware ESXi).
- **Type 2 Hypervisor**: Runs on OS (e.g., VirtualBox).

Benefits:
- **Efficiency**: Multiple VMs share resources.
- **Isolation**: Problems in one VM don’t affect others.
- **Flexibility**: Easy to create, modify, or delete VMs.

### History of Virtualization

Virtualization has evolved significantly since its inception:

- **1960s**: IBM developed virtualization for mainframe computers to run multiple operating systems, maximizing hardware utilization.
- **1990s**: Virtualization gained traction with the rise of x86 architecture. VMware was a pioneer, introducing software-based virtualization for servers and desktops.
- **2000s**: Cloud computing growth led to widespread adoption of virtualization for cost-effective resource management and scalability.
- **Present**: Virtualization is now foundational for cloud services, containerization (e.g., Docker), and orchestration platforms (e.g., Kubernetes).


## 2. Scaling: Horizontal vs. Vertical

- **Vertical Scaling**: Adding more power (CPU/RAM) to a machine.
  - **Pros**: Simple, no app changes.
  - **Cons**: Limited by machine capacity, costly.
  
- **Horizontal Scaling**: Adding more machines.
  - **Pros**: Better fault tolerance, handles more traffic.
  - **Cons**: More complex, needs distributed app design.

## 3. Threading

**Threading** allows a single process to perform multiple tasks simultaneously using separate threads.

- **Benefits**: Improved performance, responsiveness.
- **How It Works**: Threads share memory; need management to avoid conflicts.

## 4. Kubernetes and Docker

- **Docker**: Packages apps into containers for portability.
- **Kubernetes**: Orchestrates container management (deploy, scale, operate).

**Combined Benefits**:
- **Scalability**: Kubernetes scales containers based on demand.
- **Portability**: Docker containers run anywhere.

## 5. Kernel Operating Systems

- **Kernel Layer**: Core OS layer managing hardware resources.
- **Application Layer**: User-facing applications interacting with the kernel.

### Diagram:

![Kernel OS Diagram](/images/Kernel_Layout.svg.png)

## 6. The Twelve Factors

The Twelve-Factor App methodology defines best practices for building scalable and maintainable software-as-a-service (SaaS) applications:

I. **Codebase**: One codebase tracked in revision control, many deploys  
II. **Dependencies**: Explicitly declare and isolate dependencies  
III. **Config**: Store config in the environment  
IV. **Backing services**: Treat backing services as attached resources  
V. **Build, release, run**: Strictly separate build and run stages  
VI. **Processes**: Execute the app as one or more stateless processes  
VII. **Port binding**: Export services via port binding  
VIII. **Concurrency**: Scale out via the process model  
IX. **Disposability**: Maximize robustness with fast startup and graceful shutdown  
X. **Dev/prod parity**: Keep development, staging, and production as similar as possible  
XI. **Logs**: Treat logs as event streams  
XII. **Admin processes**: Run admin/management tasks as one-off processes

