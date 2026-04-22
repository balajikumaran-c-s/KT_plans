# Omnia Knowledge Transfer Plan
**Duration:** 3 weeks (starting 22-Apr-2026)  
**Target Audience:** Omnia Validation Engineer  
**Goal:** Enable independent validation of Omnia workflows

---

## Week 1: Foundations & Core Setup

| Day | Date | Topic | Owner | Duration | Activities | Validation Focus |
|-----|------|-------|--------|----------|------------|------------------|
| 1 | 22-Apr | Hardware Basics & Networking | - | 1 hr | - Server hardware components (CPU, memory, NICs, BMC)<br>- Network topology and structure<br>- BMC/iDRAC basics<br>- PXE boot concepts<br>**Hardware basics, networking, Omnia documentation walkthrough** | Understand server inventory and network structure |
| 2 | 23-Apr | Omnia Architecture Overview | - | 1 hr | - Omnia component architecture<br>- Container-based deployment<br>- Service interactions<br>- Data flow diagram<br>**Hardware basics, networking, Omnia documentation walkthrough** | System context and component understanding |
| 3 | 24-Apr | Omnia Architecture | Balaji | 1 hr | - Omnia component architecture<br>- Container-based deployment<br>- Service interactions<br>- Data flow diagram | System context and component understanding |
| 4 | 27-Apr | OS Installation & omnia.sh | Prasanth | 1 hr | - OS installation on physical servers<br>- omnia.sh script execution<br>- Environment setup<br>- Initial configuration | OS deployment and script execution validation |
| 5 | 28-Apr | prepare_oim | Prasanth | 1 hr | - OIM (Open Infrastructure Manager) deployment<br>- Credential management<br>- Service configuration<br>- Network setup | OIM deployment validation |

---

## Week 2: Building & Deployment

| Day | Date | Topic | Owner | Duration | Activities | Validation Focus |
|-----|------|-------|--------|----------|------------|------------------|
| 6 | 29-Apr | local_repo | Rohit | 1 hr | - Local repository setup<br>- Package management<br>- Pulp container role<br>- Repository endpoints | Repository validation |
| 7 | 30-Apr | build_image | Balaji | 1 hr | - Image building workflow<br>- OS image customization<br>- Template handling<br>- Registry integration | Image build validation |
| 8 | 4-May | Discovery & Provisioning | Balaji | 1 hr | - Discovery mechanisms (OME)<br>- PXE mapping file generation<br>- Provisioning workflow<br>- Node configuration | Discovery and provisioning validation |
| 9 | 5-May | K8s Cluster Deployment | Rohit | 1 hr | - Kubernetes architecture<br>- Master/worker node setup<br>- Service deployment<br>- Network configuration | K8s cluster validation |
| 10 | 6-May | Slurm Cluster Deployment | Rohit | 1 hr | - Slurm workload manager<br>- Compute/control nodes<br>- Job scheduling<br>- Service configuration | Slurm cluster validation |
| 11 | 7-May | Telemetry Workflow | Prasanth | 1 hr | - Telemetry architecture<br>- Monitoring components<br>- Data collection<br>- Metric aggregation | Telemetry validation |

---

## Week 3: Automation & Reverse KT

| Day | Date | Topic | Owner | Duration | Activities | Validation Focus |
|-----|------|-------|--------|----------|------------|------------------|
| 12 | 8-May | Automation Code Walkthrough | Balaji | 1 hr | - Ansible playbook structure<br>- Automation framework<br>- Error handling<br>- Logging mechanisms | Automation validation |
| 13 | 11-May | Reverse KT - Deployment | - | 1 hr | - Complete deployment walkthrough<br>- End-to-end validation<br>- Troubleshooting scenarios<br>- Best practices | Full deployment validation |
| 14 | 12-May | Reverse KT - Shahzama | Shahzama | 1 hr | - Deployment review with Shahzama<br>- Hands-on deployment practice<br>- Q&A session<br>- Knowledge validation | Shahzama's understanding |
| 15 | 13-May | Reverse KT - Sarvajith | Sarvajith | 1 hr | - Deployment review with Sarvajith<br>- Hands-on deployment practice<br>- Q&A session<br>- Knowledge validation | Sarvajith's understanding |

---

## Owner Responsibilities

### Balaji (Omnia Architecture, build_image, Discovery/Provisioning, Automation)
- Omnia architecture overview
- Image building workflows
- Discovery and provisioning
- Automation code walkthrough

### Prasanth (OS Installation/omnia.sh, prepare_oim, Telemetry)
- OS installation and omnia.sh execution
- OIM deployment and configuration
- Telemetry and monitoring
- Service orchestration

### Rohit (local_repo, K8s, Slurm)
- Repository management
- Kubernetes cluster deployment
- Slurm cluster deployment
- Compute node validation

### Shahzama (Reverse KT - Day 14)
- Deployment practice
- Hands-on validation
- Knowledge transfer verification

### Sarvajith (Reverse KT - Day 15)
- Deployment practice
- Hands-on validation
- Knowledge transfer verification

---

## Prerequisites & Setup

### Environment Requirements
- Access to Omnia development environment
- Test servers for validation
- Physical servers for OS installation
- Basic Linux command line knowledge

### Tools Needed
- SSH client
- Text editor
- Terminal access
- Web browser

### Pre-KT Setup Checklist
- [ ] omnia.sh script available
- [ ] Physical servers ready
- [ ] Network connectivity verified
- [ ] Test environment prepared

---

## Success Metrics

### Week 1 Goals
- Understand hardware and networking basics
- Grasp Omnia architecture
- Complete OS installation and omnia.sh execution
- Deploy OIM

### Week 2 Goals
- Deploy local_repo and build images
- Execute discovery and provisioning
- Deploy K8s and Slurm clusters
- Configure telemetry workflow

### Week 3 Goals
- Understand automation framework
- Complete reverse KT deployment
- Validate Shahzama and Sarvajith understanding

---

## Detailed Activity Breakdown

### Day 1-2 (22-23 Apr): Hardware Basics & Networking
- Review server specifications
- Understand network topology
- Learn BMC/iDRAC management
- Study PXE boot process
- **Hardware basics, networking, Omnia documentation walkthrough**

### Day 3 (24-Apr): Omnia Architecture
- Component interaction diagram
- Service dependencies
- Data flow understanding
- Container roles
- **Balaji will guide through architecture**

### Day 4 (25-Apr): OS Installation & omnia.sh
- Physical server OS setup
- omnia.sh script options
- Environment validation
- Initial configuration checks

### Day 5 (26-Apr): prepare_oim
- OIM service deployment
- Credential encryption
- Network configuration
- Service health checks

### Day 6 (29-Apr): local_repo
- Repository creation
- Package management
- Service endpoints
- Access validation

### Day 7 (30-Apr): build_image
- Image template customization
- Build process execution
- Registry interaction
- Image verification

### Day 8 (1-May): Discovery & Provisioning
- OME discovery workflow
- PXE mapping generation
- Node provisioning
- Service configuration

### Day 9 (2-May): K8s Cluster
- Master node setup
- Worker node configuration
- Service deployment
- Cluster validation

### Day 10 (3-May): Slurm Cluster
- Slurm installation
- Compute node configuration
- Job submission testing
- Cluster health checks

### Day 11 (6-May): Telemetry
- Telemetry service setup
- Data collection configuration
- Metric verification
- Reporting validation

### Day 12 (7-May): Automation
- Ansible playbook review
- Automation framework understanding
- Error handling review
- Logging mechanisms

### Day 13 (8-May): Reverse KT - Deployment
- Complete deployment review
- End-to-end workflow validation
- Troubleshooting common issues
- Best practices documentation

### Day 14 (14-May): Reverse KT - Shahzama
- Shahzama practices deployment
- Hands-on validation exercises
- Q&A for clarification
- Knowledge assessment

### Day 15 (15-May): Reverse KT - Sarvajith
- Sarvajith practices deployment
- Hands-on validation exercises
- Q&A for clarification
- Knowledge assessment

---

## Schedule Notes

- **Start Date:** 22-Apr-2026 (Tuesday)
- **Days 1-2 (22-23 Apr):** Hardware basics, networking, Omnia documentation walkthrough
- **From 24 Apr:** Omnia architecture begins with Balaji
- **Weekend:** No sessions
- **Reverse KT:** 14-May (Shahzama), 15-May (Sarvajith)
- **Total Duration:** 15 sessions over 3 weeks

---

## Reverse KT Objectives

### For Shahzama (Day 14)
- Understand complete Omnia deployment workflow
- Practice hands-on deployment
- Validate understanding through exercises
- Document questions and gaps

### For Sarvajith (Day 15)
- Understand complete Omnia deployment workflow
- Practice hands-on deployment
- Validate understanding through exercises
- Document questions and gaps

### Assessment Criteria
- Can independently navigate omnia.sh
- Can execute prepare_oim and local_repo
- Can build images and run discovery
- Can provision K8s/Slurm clusters
- Can troubleshoot common issues

---

*This plan focuses on practical Omnia deployment and validation with clear ownership and reverse KT for Shahzama and Sarvajith.*
