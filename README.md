# Sports Article CMS
<p align="center">
  <img src="./images/sports.jpeg " alt="Docker Logo" style="width:100%; max-width:600px;">
</p>

## Introduction

Welcome to the Sports Article CMS project! This platform allows users to manage, create, and publish sports articles with ease. Below you'll find a guide to get started, as well as links to more detailed documentation on different components.

---

## Table of Contents

1. [Chapter 1 - Docker](./docs/docker.md)  
   - Docker automates the deployment and management of applications by packaging them into containers. Containers ensure consistency across environments and improve efficiency by sharing the host system's resources.
2. [Chapter 2 - Containerization](./docs/containerization.md)
    - Containerization allows applications to run in isolated environments called containers, which are lightweight, efficient, and scalable by sharing the host OS kernel while maintaining their own file system, network, and process space.
3. [Chapter 3 - Kernel](./docs/kernel.md)
    - The kernel is the core of an operating system, managing hardware resources and enabling applications to interact with hardware, while the application layer consists of user-facing software that relies on the kernel to perform tasks like resource allocation, process management, and device interaction
4. [Chapter 4 - Threading](./docs/threading.md)
    - Threading allows a single process to perform multiple tasks simultaneously using separate threads, improving performance and responsiveness by sharing memory and requiring careful management to avoid conflicts like race conditions and deadlocks.
5. [Chapter 5 - Virtualization vs. Containerization](./docs/virtualizationvscontainerization.md)
    - Virtualization creates virtual machines with their own operating systems, offering strong isolation and flexibility but with higher resource use and slower performance. Containerization, on the other hand, is more lightweight and faster, sharing the host OS for efficiency, though it lacks full isolation and flexibility compared to VMs.
6. [Chapter 6 - Ubuntu For Macs](./docs/ubuntuformac.md)
    - Ubuntu is an open-source operating system popular for development. Installing it on a Mac allows you to dual-boot or switch between macOS and Ubuntu, enhancing flexibility for development work.
7. [Chapter 7 - The Twelve Factors](./docs/12factor.md)
    - The Twelve-Factor App methodology defines best practices for building scalable and maintainable SaaS applications
8. [Chapter 8 - Scaling](./docs/scaling.md)
    - Vertical scaling adds more power (CPU, RAM, storage) to a single machine, making it simple to implement but limited by capacity and cost, with a risk of downtime if the machine fails. Horizontal scaling adds more machines, improving fault tolerance and traffic handling, but requires a more complex, distributed application design.
9. [Chapter 9 - Docker vs. Kubernetes](./docs/dockervskubernetes.md)
    - Docker is simple, portable, and efficient for running containers but lacks advanced orchestration for large-scale applications. Kubernetes, though more complex, excels in managing and scaling container clusters with powerful orchestration and self-healing features.


---


## Project Files
**Note: This is a draft version of the project structure for the Sports Article CMS. It outlines the basic organization of files and pages.**
```bash
├── index.html              # Homepage with featured articles, latest news
├── categories.html         # Sports categories list
├── category.html           # Articles by category
├── article.html            # Individual article details
├── teams.html              # List of teams
├── team.html               # Team details and roster
├── players.html            # List of players
├── player.html             # Player profile
├── events.html             # Upcoming sports events
├── media.html              # Photo and video gallery
├── admin.html              # Admin dashboard
├── login.html              # Login page
├── register.html           # Registration page
├── profile.html            # User profile
├── search.html             # Search results
└── assets/
    ├── css/
    │   └── styles.css      # Main stylesheet
    ├── js/
    │   └── script.js       # Main JavaScript
    └── images/
        └── logo.png        # Site logo
