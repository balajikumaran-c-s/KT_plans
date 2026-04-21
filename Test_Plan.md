# Omnia Knowledge Transfer Plan
**Duration:** 3 weeks (1 hour daily)  
**Target Audience:** Omnia Validation Engineer  
**Goal:** Enable independent validation of Omnia workflows

---

## Week 1: Foundations & Core Setup

| Day | Topic | Owner | Duration | Activities | Hands-on | Validation Focus |
|-----|-------|--------|----------|------------|----------|------------------|
| 1 | Server Basics Overview | - | 1 hr | - Server hardware components (CPU, memory, NICs, BMC)<br>- BMC/iDRAC basics<br>- PXE boot concepts | Identify BMC IPs in lab | Understand server inventory |
| 2 | omnia.sh Script Deep Dive | Balaji | 1 hr | - Script structure and options<br>- Environment setup<br>- Logging and troubleshooting | Run `./omnia.sh --help`<br>Check logs | Script navigation |
| 3 | prepare_oim - Theory | Prasanth | 1 hr | - OIM (Open Infrastructure Manager) role<br>- Credential management<br>- Network configuration prerequisites | Review prepare_oim.yml | Understand prerequisites |
| 4 | prepare_oim - Hands-on | Prasanth | 1 hr | - Run prepare_oim playbook<br>- Verify OIM services<br>- Check credential encryption | Execute playbook<br>Validate services | OIM deployment validation |
| 5 | local_repo - Theory | Rohit | 1 hr | - Local repository purpose<br>- Package management<br>- Pulp container role | Review local_repo.yml | Repository concepts |
| 6 | local_repo - Hands-on | Rohit | 1 hr | - Run local_repo playbook<br>- Verify repo endpoints<br>- Test package access | Execute playbook<br>Browse repos | Repository validation |
| 7 | build_image - Theory | Balaji | 1 hr | - Image building workflow<br>- OS image customization<br>- Integration with local_repo | Review build_image.yml | Image build concepts |

---

## Week 2: Image Building & Build Stream

| Day | Topic | Owner | Duration | Activities | Hands-on | Validation Focus |
|-----|-------|--------|----------|------------|----------|------------------|
| 8 | build_image - Hands-on | Balaji | 1 hr | - Run build_image playbook<br>- Verify image artifacts<br>- Check image registry | Execute playbook<br>List images | Image build validation |
| 9 | build_stream - Theory | Balaji | 1 hr | - Build stream workflow<br>- Stream configuration<br>- Integration with core container | Read build_stream playbooks<br>Check core container | Build stream concepts |
| 10 | build_stream - Hands-on | Balaji | 1 hr | - Configure build stream<br>- Execute stream build<br>- Verify stream output | Run build_stream<br>Check results | Build stream validation |
| 11 | provision.yml Overview | Balaji | 1 hr | - Provisioning workflow<br>- Node configuration<br>- Integration points | Review provision.yml | Provisioning understanding |
| 12 | Slurm Provisioning | Rohit | 1 hr | - Slurm architecture<br>- Compute/control node roles<br>- Service configuration | Plan Slurm deployment | Slurm validation prep |
| 13 | Kubernetes Basics | Prasanth | 1 hr | - K8s components<br>- Master/worker roles<br>- Network requirements | Read K8s playbooks | K8s concepts |
| 14 | Telemetry Overview | Prasanth | 1 hr | - Telemetry architecture<br>- Monitoring components<br>- Data collection | Review telemetry playbooks | Telemetry concepts |

---

## Week 3: Code Review & Validation

| Day | Topic | Owner | Duration | Activities | Hands-on | Validation Focus |
|-----|-------|--------|----------|------------|----------|------------------|
| 15 | Code Review - omnia.sh | Balaji | 1 hr | - Script structure analysis<br>- Error handling<br>- Logging mechanisms | Read omnia.sh code | Script validation |
| 16 | Code Review - prepare_oim | Prasanth | 1 hr | - Playbook structure<br>- Role dependencies<br>- Configuration validation | Read prepare_oim playbooks | OIM validation |
| 17 | Code Review - local_repo | Rohit | 1 hr | - Repository management<br>- Package handling<br>- Service configuration | Read local_repo playbooks | Repo validation |
| 18 | Code Review - build_image | Balaji | 1 hr | - Image build process<br>- Template handling<br>- Registry integration | Read build_image playbooks | Build validation |
| 19 | Code Review - provision | Balaji | 1 hr | - Node provisioning<br>- Service setup<br>- Configuration management | Read provision playbooks | Provision validation |
| 20 | Code Review - K8s & Telemetry | Prasanth | 1 hr | - K8s deployment playbooks<br>- Telemetry collection<br>- Service integration | Read K8s/telemetry code | Service validation |
| 21 | Validation Best Practices | All | 1 hr | - Test case design for Omnia<br>- Automation approaches<br>- Reporting standards | Review validation strategy | Validation methodology |

---

## Daily Structure Template

### First 15 minutes: Review
- Previous day concepts
- Questions and clarifications
- Progress check

### Next 30 minutes: Theory/Demo
- Concept explanation
- Live demonstration
- Code/architecture review

### Final 15 minutes: Hands-on Practice
- Guided exercises
- Independent practice
- Next day preparation

---

## Owner Responsibilities

### Balaji (omnia.sh, build_image, build_stream, provision)
- Core script functionality
- Image building workflows
- Build stream configuration
- Node provisioning

### Prasanth (prepare_oim, K8s, telemetry)
- OIM deployment and configuration
- Kubernetes components
- Telemetry and monitoring
- Service orchestration

### Rohit (local_repo, Slurm)
- Repository management
- Package distribution
- Slurm workload manager
- Compute node validation

---

## Prerequisites & Setup

### Environment Requirements
- Access to Omnia development environment
- Test servers for validation
- omnia_core container access
- Basic Linux command line knowledge

### Tools Needed
- SSH client
- Text editor
- Terminal access
- Web browser

### Pre-KT Setup Checklist
- [ ] omnia.sh script available
- [ ] Test environment ready
- [ ] Network connectivity verified
- [ ] Documentation access

---

## Success Metrics

### Week 1 Goals
- Understand Omnia architecture
- Successfully run prepare_oim
- Verify local_repo deployment
- Navigate omnia_core container

### Week 2 Goals
- Build custom images
- Execute build_stream
- Understand provisioning workflow
- Grasp K8s and telemetry basics

### Week 3 Goals
- Read and understand core playbooks
- Identify validation points
- Document validation strategies
- Prepare for independent validation

---

## Code Review Focus Areas

### omnia.sh (Balaji)
- Script entry points
- Environment validation
- Error handling
- Logging mechanisms

### prepare_oim (Prasanth)
- OIM service deployment
- Credential management
- Network configuration
- Service dependencies

### local_repo (Rohit)
- Repository setup
- Package management
- Service endpoints
- Access validation

### build_image (Balaji)
- Image templates
- Build process
- Registry interaction
- Customization options

### build_stream (Balaji)
- Stream configuration
- Build orchestration
- Output handling
- Integration points

### provision (Balaji)
- Node provisioning
- Service configuration
- Role assignment
- Post-provision validation

### K8s (Prasanth)
- Cluster deployment
- Service configuration
- Network setup
- Pod management

### Telemetry (Prasanth)
- Data collection
- Service monitoring
- Metric aggregation
- Reporting

---

*This plan focuses on understanding Omnia codebase and workflows for validation purposes, with clear ownership and hands-on code review.*
