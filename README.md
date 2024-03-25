# Homemade Container From Scratch

The Homemade Container From Scratch project is an educational endeavor aimed at demystifying the world of containers by building a simple container from scratch using Golang and Linux namespaces for process isolation. This project serves as a hands-on exploration of containerization concepts, including process isolation, namespace manipulation, and resource control.

## Features

### 1. Process Isolation with Linux Namespaces
The container implements process isolation using various Linux namespaces, including:
- PID (Process ID) Namespace: Provides isolation for process IDs, allowing processes inside the container to have their own PID namespace independent from the host.
- UTS (Unix Timesharing System) Namespace: Isolates hostname and domain name identifiers, enabling the container to have its own hostname.
- Mount Namespace: Isolates filesystem mounts, enabling the container to have its own root filesystem and mount points.

### 2. Basic Container Functionality
The container supports basic functionality such as running commands inside the container environment. Users can specify the command to execute when creating a container instance.

### 3. Potential Improvement: Integration with cgroups
While not implemented in the current version, integrating with cgroups (control groups) could be a potential improvement. Cgroups enable resource isolation and control, allowing for better management of CPU, memory, and other system resources for containers.

## Getting Started

To run the Homemade Container From Scratch project, follow these steps:

1. Clone the repository:
https://github.com/haitammabrouk/homemade-container

2. Navigate to the project directory
3. Build the project: go build
4. Run the container: go run main.go run sh
