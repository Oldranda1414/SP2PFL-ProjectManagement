Once the POS is approved, the Planning phase can start.

## Joint Project Planning Sessions

Joint Project Planning Sessions (JPPSs) are scheduled. The entire development team and project manager will partecipate to these meetings.

The PM schedules and organizes the meetings deciding:

- Attendees:
    - The entire development team (14 members), Finance Manager, Customer Experience Analyst and the PM himself
- Facilities:
    - The meeting room in OpenML offices is spacious enough for the JPPSs to take place
- Equipment:
    - The meeting room provides a wide round table with enough seats for all attendees
    - Office laptops and pen and paper will be provided

### Agenda

The following Agenda will be carried out throughout the JPPSs

1. Introduction
    - Introduction of attendees
    - Introduction of project
    - Introduction of the agenda
2. Project Analysis
    - Develop of Work Breakdown Structure
    - Construct of Dependency Diagram
    - Construct of Network Diagram
    - Schedule Compression
3. Risk and Resource Planning
    - Risk Assessment
    - Resource Allocation
4. Documentation
    - Draft of Project Definition Statement
    - Writing of Project Proposal
    - Summarise Project Notebook

### Deliverables

The deliverables expected to be produced at the end of the meetings are:

- Project Definition Statement (PDS)
- Work Breakdown Structure (WBS)
- Required Resources
- Resource Allocation
- Estimate Activity Duration
- Project Network Schedule
- Activity Scheduling
- Project Notebook
- Project Proposal

## Work Breakdown Structure

Activities are constructed to represent the work to be done to satisfy the requirements expressed by the user stories.

Since the relationship between user stories and activities is non trivial Requirements Traceability Matrixes (RTM) are used to highlight these relationships.

Since some activities are totally fully they do not have a user story related.

### Research & Design

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 1.1 | Study and interpret the Secure Average Computation algorithm (Wink et al., 2021) | 3.3.2.1 |
| 1.2 | Design federated architecture (server–peer topology, communication flow) | 3.3.1.2 |
| 1.3 | Define security and encryption mechanisms for peer communication | 3.2.1.1, 3.2.1.2, 3.2.1.3 |
| 1.4 | Define API specifications and endpoints | 1.1.3.1, 3.1.1.3, 3.1.3.2, 3.1.4.4, 3.3.1.6, 3.3.3.4, 4.2.1.1 |
| 1.5 | Design data schema and metadata format for federated datasets | 2.1.1.1, 2.1.1.2, 2.1.3.2 |
| 1.6 | Produce software architecture documentation and design diagrams | |
| 1.7 | Validate design through technical review | |

### Core Framework Development

#### Core

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 2.1.1 | Implement peer registration and authentication subsystem | 1.2.2.1, 3.1.1.1, 3.1.1.2, 3.1.1.3, 3.2.1.5 |
| 2.1.2 | Develop data preprocessing interface and function library | 2.1.2.1, 2.1.2.2, 2.1.2.3 |
| 2.1.3 | Implement role and permission management | 3.1.2.1, 3.1.2.2, 3.1.2.3, 3.1.3.1, 3.1.3.2, 3.1.3.3, 4.1.2.1, 4.1.2.2, 4.1.2.3, 4.1.2.4, 4.1.2.5 |
| 2.1.4 | Implement federated orchestration service (task coordination, scheduling) | 3.3.1.1, 3.3.1.2, 3.3.1.3, 3.3.1.4, 3.3.1.5 |
| 2.1.5 | Develop Secure Average Computation module | 3.3.2.2 |
| 2.1.6 | Implement communication protocol for distributed training | 3.2.2.1, 3.2.2.2, 3.2.2.3, 3.2.2.4, 3.2.2.5, 3.2.2.6 |
| 2.1.7 | Develop API endpoints for peer and admin operations | 1.1.3.1, 2.1.1.3, 2.3.1.3, 2.3.2.3, 2.3.3.4, 3.3.3.4, 4.2.1.1, 4.2.1.2, 4.2.1.4 |
| 2.1.8 | Integrate monitoring and logging capabilities | 1.3.3.2, 2.1.3.3, 3.2.1.6, 3.2.1.7, 3.2.4.1, 3.2.4.2, 3.2.4.3, 3.2.4.4, 3.2.4.5, 3.2.4.6, 3.3.3.5, 4.1.2.2, 4.1.3.5, 4.2.1.5, 4.2.3.5 |
| 2.1.9 | Conduct unit and integration testing for modules | |

#### Model Definition & Configuration

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 2.2.1 | Design and implement input schema definition system | 2.1.1.1, 2.1.1.2, 2.1.1.3 |
| 2.2.2 | Create layer configuration interface (UI and API) | 2.2.1.1, 2.2.1.2, 2.2.1.3 |
| 2.2.3 | Build supported architectures library and templates | 2.2.2.1, 2.2.2.2, 2.2.2.3 |
| 2.2.4 | Implement model architecture validation system | 2.2.3.1, 2.2.3.2, 2.2.3.3 |
| 2.2.5 | Develop custom layer support with sandboxing | 2.2.4.1, 2.2.4.2, 2.2.4.3, 3.3.2.4, 3.3.2.5 |
| 2.2.6 | Design and implement output schema definition system | 2.3.1.1, 2.3.1.2, 2.3.1.3 |
| 2.2.7 | Develop model export and serialization capabilities | 2.3.2.1, 2.3.2.2, 2.3.2.3, 4.2.2.1, 4.2.2.2 |
| 2.2.8 | Implement evaluation and metrics interface | 2.3.3.1, 2.3.3.2, 2.3.3.3, 2.3.3.4 |
| 2.2.9 | Conduct unit and integration testing for modules | |

#### Federation Management & Security

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 2.3.1 | Implement membership lifecycle management system | 3.1.4.1, 3.1.4.2, 3.1.4.3, 3.1.4.4 |
| 2.3.2 | Develop secure communication layer with TLS/mTLS | 3.2.1.1, 3.2.1.2, 3.2.1.3, 3.2.1.4 |
| 2.3.3 | Implement certificate management and auto-renewal | 3.2.1.4 |
| 2.3.4 | Build authentication and identity management system | 3.2.1.5, 3.2.1.6, 3.2.1.7 |
| 2.3.5 | Develop fault tolerance and retry mechanisms | 3.2.3.1, 3.2.3.2, 3.2.3.3, 3.2.3.4, 3.2.3.5, 3.2.3.6 |
| 2.3.6 | Implement aggregation strategy framework | 3.3.2.1, 3.3.2.2, 3.3.2.3, 3.3.2.4, 3.3.2.5, 3.3.2.6 |
| 2.3.7 | Develop training error handling and recovery system | 3.3.4.1, 3.3.4.2, 3.3.4.3, 3.3.4.4, 3.3.4.5, 3.3.4.6 |
| 2.3.8 | Conduct unit and integration testing for modules | |

#### Model Storage & Inference

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 2.4.1 | Implement model version control system | 4.1.1.1, 4.1.1.2, 4.1.1.3, 4.1.1.4, 4.1.1.5 |
| 2.4.2 | Develop model access control and permission system | 4.1.2.1, 4.1.2.2, 4.1.2.3, 4.1.2.4, 4.1.2.5 |
| 2.4.3 | Implement model integrity verification system | 4.1.3.1, 4.1.3.2, 4.1.3.3, 4.1.3.4, 4.1.3.5 |
| 2.4.4 | Build inference API service with batch processing | 4.2.1.1, 4.2.1.2, 4.2.1.3, 4.2.1.4, 4.2.1.5, 4.2.1.6 |
| 2.4.5 | Develop edge deployment and optimization system | 4.2.2.1, 4.2.2.2, 4.2.2.3, 4.2.2.4, 4.2.2.5, 4.2.2.6 |
| 2.4.6 | Implement performance monitoring and analytics | 4.2.3.1, 4.2.3.2, 4.2.3.3, 4.2.3.4, 4.2.3.5, 4.2.3.6 |
| 2.4.7 | Develop model update and deployment orchestration | 4.2.4.1, 4.2.4.2, 4.2.4.3, 4.2.4.4, 4.2.4.5, 4.2.4.6 |
| 2.4.8 | Conduct unit and integration testing for modules | |

### Infrastructure & Deployment

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 3.1 | Configure development and testing environments | 1.2.1.3 |
| 3.2 | Implement containerization (e.g., Docker) for peer and server components | 1.1.2.2 |
| 3.3 | Set up orchestration (Kubernetes or similar) | 1.1.2.2, 4.2.1.3, 4.2.4.1 |
| 3.4 | Create CI/CD pipelines for automated builds and deployment | 1.2.1.3 |
| 3.5 | Configure cloud infrastructure for distributed experiments | |
| 3.6 | Establish data privacy and network security policies | 3.2.1.3 |
| 3.7 | Deploy framework to production (SAAS hosting) | 1.2.1.1, 1.2.1.2, 1.2.1.3, 3.1.1.2 |
| 3.8 | Conduct scalability and performance tests | 4.2.1.3, 4.2.1.6 |

### Federated Learning Integration

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 4.1 | Implement model aggregation logic using Secure Average Computation | 3.3.2.1, 3.3.2.2, 3.3.2.3 |
| 4.2 | Define model update serialization and exchange protocol | 3.2.2.1, 3.2.2.2, 3.2.2.3 |
| 4.3 | Handle asynchronous peer updates and dropout resilience | 3.2.3.1, 3.2.3.2, 3.2.3.3, 3.2.3.4, 3.2.3.5, 3.2.3.6, 3.3.4.1, 3.3.4.3, 3.3.4.4 |
| 4.4 | Implement audit trail and logging of training rounds | 3.1.4.3, 3.2.4.1, 3.2.4.2, 3.3.3.5 |
| 4.5 | Integrate algorithm with orchestration and monitoring services | 3.3.1.5, 3.3.3.1, 3.3.3.2, 3.3.3.3 |
| 4.6 | Validate model performance and convergence under federation | 1.3.3.1, 3.3.4.6 |

### User Interface & Experience

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 5.1 | Design admin dashboard (federation overview, peer management) | 1.1.1.2, 1.2.2.3, 1.3.1.2, 1.3.2.3, 3.1.1.1, 3.1.2.1, 3.1.4.1, 3.2.4.6, 3.3.1.1, 3.3.1.5, 3.3.3.3, 4.1.1.4, 4.2.3.2, 4.2.3.4 |
| 5.2 | Design peer organization dashboard (local training, participation status) | 1.3.3.1, 2.3.1.2, 2.3.3.3, 3.1.2.2, 3.1.4.2, 3.3.3.2, 4.1.1.1, 4.1.1.2 |
| 5.3 | Implement role-based access controls in the UI | 3.1.2.1, 3.1.2.2, 3.1.3.1, 4.1.2.1, 4.1.2.3 |
| 5.4 | Integrate credential management and registration flows | 1.3.1.1, 3.1.1.2 |
| 5.5 | Add notifications for federation events and status updates | 1.2.2.3, 3.3.3.6, 4.2.3.3 |
| 5.6 | Conduct usability testing and collect feedback | 1.1.1.1, 1.3.1.3 |
| 5.7 | Implement help, documentation, and onboarding pages | 1.1.1.1, 1.1.2.1, 1.1.3.1, 1.1.3.2, 1.3.1.1 |

### Quality Assurance & Documentation

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 6.1 | Develop comprehensive test plan (unit, integration, system, acceptance) | 1.2.1.3, 2.2.3.2, 3.3.2.6, 4.2.4.4 |
| 6.2 | Perform security and compliance testing | 1.2.2.1, 2.2.4.2, 3.1.3.3, 3.1.4.3, 3.2.4.1, 4.1.1.5, 4.1.3.1, 4.2.1.4, 4.2.2.4, 4.2.4.5 |
| 6.3 | Conduct performance benchmarking | 2.2.4.3, 3.2.2.4, 3.2.2.5, 4.2.1.3, 4.2.3.1 |
| 6.4 | Maintain traceability between user stories and test cases | 1.1.1.3, 1.3.3.3 |
| 6.5 | Prepare technical documentation (API docs, deployment guide) | 1.1.2.2, 1.1.2.3, 1.1.3.1, 1.3.2.2, 3.3.2.5 |
| 6.6 | Write user documentation and quick-start manuals | 1.1.2.1, 1.1.3.2, 1.1.3.3, 1.2.1.1, 1.2.1.2 |
| 6.7 | Conduct final validation and acceptance testing | 1.2.2.2 |
| 6.8 | Prepare lessons learned and project closure report | |

## Resource Allocation

### Human Resources

| Role | Count | Primary Focus Areas |
|------|-------|---------------------|
| Project Managers | 1 | Overall coordination, timeline, budget |
| ML Research Leads | 2 | Research & Design, Algorithm validation |
| Senior Backend Engineers | 2 | Core Framework, Federation Management |
| DevOps Engineers | 2 | Infrastructure & Deployment |
| ML Engineers | 2 | Federated Learning Integration, Model Definition |
| Frontend Engineers | 2 | User Interface & Experience |
| QA Engineers | 2 | Quality Assurance & Documentation |
| Full-stack Engineers | 2 | Model Storage & Inference |

Most roles are covered by at least two employees to enable code review sessions and limit the risk of optimistic predictions.

### Infrastructure & Tools

| Category | Resources | Purpose |
|----------|-----------|---------|
| Development | 3x AWS EC2 instances, GitHub Teams | Core development and version control |
| Testing | Kubernetes cluster, 5x test peer nodes | Integration and federation testing |
| Staging | Scaled-down production environment | Pre-production validation |
| Production | Multi-region Kubernetes, 50+ peer capacity | SAAS hosting and client deployments |
| Monitoring | Prometheus | Performance and security monitoring |

Known tools were preferred to limit employee training necessity.

### Budget Allocation

| Area | Percentage | Description |
|------|------------|-------------|
| Personnel | 65% | Salaries for 15-person team |
| Infrastructure | 20% | Cloud services, development tools |
| Security & Compliance | 10% | Audits, penetration testing, certifications |
| Contingency | 5% | Unplanned expenses, scope changes |

Percentage estimations have been aided by past project experience.

## Activity Durations & Dependencies

Given the allocated resources, the following activity dependecies and estimate durations have been considered.

| ID | Duration Estimate | Dependencies |
|----|------------------|--------------|
| 1.1 | 3 weeks | - |
| 1.2 | 2 weeks | 1.1 |
| 1.3 | 2 weeks | 1.2 |
| 1.4 | 3 weeks | 1.2 |
| 1.5 | 2 weeks | 1.2 |
| 1.6 | 1 week | 1.3, 1.4, 1.5 |
| 1.7 | 1 week | 1.6 |
| 2.1.1 | 4 weeks | 6.4 |
| 2.1.2 | 3 weeks | 6.4 |
| 2.1.3 | 5 weeks | 2.1.1 |
| 2.1.4 | 6 weeks | 2.1.1 |
| 2.1.5 | 4 weeks | 6.4 |
| 2.1.6 | 5 weeks | 6.4 |
| 2.1.7 | 6 weeks | 2.1.3 |
| 2.1.8 | 4 weeks | 2.1.4, 2.1.6 |
| 2.1.9 | 3 weeks | 2.1.2, 2.1.3, 2.1.5, 2.1.7, 2.1.8 |
| 2.2.1 | 3 weeks | 6.4 |
| 2.2.2 | 3 weeks | 2.2.1 |
| 2.2.3 | 4 weeks | 2.2.1 |
| 2.2.4 | 3 weeks | 2.2.2, 2.2.3 |
| 2.2.5 | 4 weeks | 2.2.4 |
| 2.2.6 | 2 weeks | 2.2.1 |
| 2.2.7 | 4 weeks | 2.2.4, 2.2.6 |
| 2.2.8 | 3 weeks | 2.2.6 |
| 2.2.9 | 2 weeks | 2.2.5, 2.2.7, 2.2.8 |
| 2.3.1 | 3 weeks | 2.1.1 |
| 2.3.2 | 4 weeks | 6.4 |
| 2.3.3 | 2 weeks | 2.3.2 |
| 2.3.4 | 5 weeks | 2.1.1, 2.3.2 |
| 2.3.5 | 4 weeks | 2.1.4, 2.3.2 |
| 2.3.6 | 5 weeks | 2.1.5 |
| 2.3.7 | 4 weeks | 2.3.5, 2.3.6 |
| 2.3.8 | 2 weeks | 2.3.1, 2.3.3, 2.3.4, 2.3.7 |
| 2.4.1 | 4 weeks | 2.2.7 |
| 2.4.2 | 3 weeks | 2.1.3, 2.4.1 |
| 2.4.3 | 3 weeks | 2.4.1 |
| 2.4.4 | 6 weeks | 2.2.7, 2.2.8 |
| 2.4.5 | 5 weeks | 2.4.1 |
| 2.4.6 | 4 weeks | 2.1.8, 2.4.4 |
| 2.4.7 | 5 weeks | 2.4.1, 2.4.5 |
| 2.4.8 | 3 weeks | 2.4.2, 2.4.3, 2.4.6, 2.4.7 |
| 3.1 | 2 weeks | 6.4 |
| 3.2 | 3 weeks | 3.1 |
| 3.3 | 4 weeks | 3.2 |
| 3.4 | 3 weeks | 3.3 |
| 3.5 | 2 weeks | 3.3 |
| 3.6 | 1 week | 6.4 |
| 3.7 | 2 weeks | 3.4, 3.5, 3.6 |
| 3.8 | 3 weeks | 3.7 |
| 4.1 | 4 weeks | 2.1.5, 2.3.6 |
| 4.2 | 3 weeks | 2.2.7, 2.1.6 |
| 4.3 | 5 weeks | 2.3.5, 4.1, 4.2 |
| 4.4 | 2 weeks | 2.1.8, 4.3 |
| 4.5 | 4 weeks | 2.1.4, 4.4 |
| 4.6 | 3 weeks | 4.5 |
| 5.1 | 6 weeks | 2.1.4, 2.1.7 |
| 5.2 | 5 weeks | 2.1.7, 2.2.2 |
| 5.3 | 3 weeks | 2.1.3, 5.1, 5.2 |
| 5.4 | 2 weeks | 2.3.4, 5.1, 5.2 |
| 5.5 | 2 weeks | 2.1.8, 5.1, 5.2 |
| 5.6 | 2 weeks | 5.3, 5.4, 5.5 |
| 5.7 | 3 weeks | 5.6 |
| 6.1 | 2 weeks | 1.7 |
| 6.2 | 4 weeks | 2.3.8, 3.7 |
| 6.3 | 3 weeks | 3.8, 4.6 |
| 6.4 | 1 week | 6.1 |
| 6.5 | 4 weeks | 2.1.9, 2.2.9, 2.3.8, 2.4.8, 3.7 |
| 6.6 | 3 weeks | 5.7, 6.5 |
| 6.7 | 2 weeks | 6.2, 6.3, 6.6 |
| 6.8 | 1 week | 6.7 |

By considering activity dependencies and slacks the Project Network Diagram has been produced.

## Project Network Diagram

NOTE Due to the rendering engine the following graphs are best seen in light mode.

### Research & Design

```mermaid
graph TD
    %% Activities
    1.1:::research
    1.2:::research
    1.3:::research
    1.4:::research
    1.5:::research
    1.6:::research
    1.7:::research
    6.1:::qa

    %% Dependencies
    1.1 --> 1.2
    1.2 --> 1.3
    1.2 --> 1.4
    1.2 --> 1.5
    1.3 --> 1.6
    1.4 --> 1.6
    1.5 --> 1.6
    1.6 --> 1.7
    1.7 --> 6.1

    classDef research fill:#d4e6ff,stroke:#3366cc,stroke-width:2px
    classDef qa fill:#f2e6d9,stroke:#b38c5c,stroke-width:2px
```

The Critical Path for these activities is:

**1.1 --> 1.2 --> 1.4 --> 1.6 --> 1.7**

This path has an estimated total duration of 10 weeks.

### Core

```mermaid
graph TD
    %% Activities
    2.1.1:::core
    2.1.2:::core
    2.1.3:::core
    2.1.4:::core
    2.1.5:::core
    2.1.6:::core
    2.1.7:::core
    2.1.8:::core
    2.1.9:::core
    6.4:::qa

    %% Dependencies
    6.4 --> 2.1.1
    6.4 --> 2.1.2
    6.4 --> 2.1.5
    6.4 --> 2.1.6
    
    2.1.1 --> 2.1.3
    2.1.1 --> 2.1.4
    2.1.3 --> 2.1.7
    2.1.2 --> 2.1.9
    2.1.4 --> 2.1.8
    2.1.5 --> 2.1.9
    2.1.6 --> 2.1.8
    2.1.7 --> 2.1.9
    2.1.8 --> 2.1.9

    classDef core fill:#d4f7d4,stroke:#2d862d,stroke-width:2px
    classDef qa fill:#f2e6d9,stroke:#b38c5c,stroke-width:2px
```

The Critical Path for these activities is:

**2.1.1 --> 2.1.3 --> 2.1.7 --> 2.1.9**

This path has an estimated total duration of 17 weeks.

### Model Definition & Configuration

```mermaid
graph TD
    %% Activities
    2.2.1:::model
    2.2.2:::model
    2.2.3:::model
    2.2.4:::model
    2.2.5:::model
    2.2.6:::model
    2.2.7:::model
    2.2.8:::model
    2.2.9:::model
    6.4:::qa

    %% Dependencies
    6.4 --> 2.2.1
    2.2.1 --> 2.2.2
    2.2.1 --> 2.2.3
    2.2.1 --> 2.2.6
    2.2.2 --> 2.2.4
    2.2.3 --> 2.2.4
    2.2.4 --> 2.2.5
    2.2.4 --> 2.2.7
    2.2.5 --> 2.2.9
    2.2.6 --> 2.2.7
    2.2.6 --> 2.2.8
    2.2.7 --> 2.2.9
    2.2.8 --> 2.2.9

    classDef model fill:#e6f7e6,stroke:#45a045,stroke-width:2px
    classDef qa fill:#f2e6d9,stroke:#b38c5c,stroke-width:2px
```

The Critical Path for these activities is:

**2.2.1 --> 2.2.3 --> 2.2.4 --> 2.2.5/2.2.7 --> 2.2.9**

This path has an estimated total duration of 17 weeks.

### Federation Management & Security

```mermaid
graph TD
    %% Activities
    2.1.1:::core
    2.1.4:::core
    2.1.5:::core
    2.3.1:::security
    2.3.2:::security
    2.3.3:::security
    2.3.4:::security
    2.3.5:::security
    2.3.6:::security
    2.3.7:::security
    2.3.8:::security
    6.4:::qa
    
    %% Dependencies
    6.4 --> 2.3.2
    2.1.1 --> 2.3.1
    2.1.1 --> 2.3.4
    2.1.4 --> 2.3.5
    2.1.5 --> 2.3.6
    2.3.1 --> 2.3.8
    2.3.2 --> 2.3.3
    2.3.2 --> 2.3.4
    2.3.2 --> 2.3.5
    2.3.3 --> 2.3.8
    2.3.4 --> 2.3.8
    2.3.5 --> 2.3.7
    2.3.6 --> 2.3.7
    2.3.7 --> 2.3.8

    classDef core fill:#d4f7d4,stroke:#2d862d,stroke-width:2px
    classDef security fill:#f0f7e6,stroke:#8cb84d,stroke-width:2px
    classDef qa fill:#f2e6d9,stroke:#b38c5c,stroke-width:2px
```

The Critical Path for these activities is:

**2.3.2 --> 2.3.5 --> 2.3.7 --> 2.3.8**

This path has an estimated total duration of 14 weeks.

### Model Storage & Inference

```mermaid
graph TD
    %% Activities
    2.1.3:::core
    2.1.8:::core
    2.2.7:::model
    2.2.8:::model
    2.4.1:::storage
    2.4.2:::storage
    2.4.3:::storage
    2.4.4:::storage
    2.4.5:::storage
    2.4.6:::storage
    2.4.7:::storage
    2.4.8:::storage

    %% Dependencies
    2.1.3 --> 2.4.2
    2.1.8 --> 2.4.6
    2.2.7 --> 2.4.1
    2.2.7 --> 2.4.4
    2.2.8 --> 2.4.4
    2.4.1 --> 2.4.2
    2.4.1 --> 2.4.3
    2.4.1 --> 2.4.5
    2.4.2 --> 2.4.8
    2.4.3 --> 2.4.8
    2.4.4 --> 2.4.6
    2.4.5 --> 2.4.7
    2.4.6 --> 2.4.8
    2.4.7 --> 2.4.8

    classDef core fill:#d4f7d4,stroke:#2d862d,stroke-width:2px
    classDef model fill:#e6f7e6,stroke:#45a045,stroke-width:2px
    classDef storage fill:#e6f7f0,stroke:#45a08c,stroke-width:2px
```

The Critical Path for these activities is:

**2.4.1 --> 2.4.5 --> 2.4.7 --> 2.4.8**

This path has an estimated total duration of 17 weeks.

### Infrastructure & Deployment

```mermaid
graph TD
    %% Activities
    3.1:::infra
    3.2:::infra
    3.3:::infra
    3.4:::infra
    3.5:::infra
    3.6:::infra
    3.7:::infra
    3.8:::infra
    6.4:::qa

    %% Dependencies
    6.4 --> 3.1
    6.4 --> 3.6
    3.1 --> 3.2
    3.2 --> 3.3
    3.3 --> 3.4
    3.3 --> 3.5
    3.4 --> 3.7
    3.5 --> 3.7
    3.6 --> 3.7
    3.7 --> 3.8

    classDef infra fill:#fff2cc,stroke:#e6ac00,stroke-width:2px
    classDef qa fill:#f2e6d9,stroke:#b38c5c,stroke-width:2px
```

The Critical Path for these activities is:

**3.1 --> 3.2 --> 3.3 --> 3.4/3.5 --> 3.7 --> 3.8**

This path has an estimated total duration of 17 weeks.

### Federated Learning Integration

```mermaid
graph TD
    %% Activities
    2.1.4:::core
    2.1.5:::core
    2.1.6:::core
    2.1.8:::core
    2.2.7:::model
    2.3.5:::security
    2.3.6:::security
    4.1:::fl
    4.2:::fl
    4.3:::fl
    4.4:::fl
    4.5:::fl
    4.6:::fl
    
    %% Dependencies
    2.1.4 --> 4.5
    2.1.5 --> 4.1
    2.1.6 --> 4.2
    2.1.8 --> 4.4
    2.2.7 --> 4.2
    2.3.5 --> 4.3
    2.3.6 --> 4.1
    4.1 --> 4.3
    4.2 --> 4.3
    4.3 --> 4.4
    4.4 --> 4.5
    4.5 --> 4.6

    classDef core fill:#d4f7d4,stroke:#2d862d,stroke-width:2px
    classDef model fill:#e6f7e6,stroke:#45a045,stroke-width:2px
    classDef security fill:#f0f7e6,stroke:#8cb84d,stroke-width:2px
    classDef fl fill:#e6e6ff,stroke:#6666ff,stroke-width:2px
```

The Critical Path for these activities is:

**4.1 --> 4.3 --> 4.4 --> 4.5 --> 4.6**

This path has an estimated total duration of 18 weeks.

### User Interface & Experience

```mermaid
graph TD
    %% Activities
    2.1.3:::core
    2.1.4:::core
    2.1.7:::core
    2.1.8:::core
    2.2.2:::model
    2.3.4:::security
    5.1:::ui
    5.2:::ui
    5.3:::ui
    5.4:::ui
    5.5:::ui
    5.6:::ui
    5.7:::ui

    %% Dependencies
    2.1.3 --> 5.3
    2.1.4 --> 5.1
    2.1.7 --> 5.1
    2.1.7 --> 5.2
    2.1.8 --> 5.5
    2.2.2 --> 5.2
    2.3.4 --> 5.4
    5.1 --> 5.3
    5.1 --> 5.4
    5.1 --> 5.5
    5.2 --> 5.3
    5.2 --> 5.4
    5.2 --> 5.5
    5.3 --> 5.6
    5.4 --> 5.6
    5.5 --> 5.6
    5.6 --> 5.7
    
    %%% UI/UX Dependencies

    classDef core fill:#d4f7d4,stroke:#2d862d,stroke-width:2px
    classDef model fill:#e6f7e6,stroke:#45a045,stroke-width:2px
    classDef security fill:#f0f7e6,stroke:#8cb84d,stroke-width:2px
    classDef ui fill:#ffe6f2,stroke:#cc66a3,stroke-width:2px
```

The Critical Path for these activities is:

**5.1 --> 5.3 --> 5.6 --> 5.7**

This path has an estimated total duration of 14 weeks.

### Quality Assurance & Documentation

```mermaid
graph TD
    %% Activities
    1.7:::research
    2.1.9:::core
    2.2.9:::model
    2.3.8:::security
    2.4.8:::storage
    3.7:::infra
    3.8:::infra
    4.6:::fl
    5.7:::ui
    6.1:::qa
    6.2:::qa
    6.3:::qa
    6.4:::qa
    6.5:::qa
    6.6:::qa
    6.7:::qa
    6.8:::qa
    
    %% Dependencies
    1.7 --> 6.1
    6.1 --> 6.4

    2.1.9 --> 6.5
    2.2.9 --> 6.5
    2.3.8 --> 6.2
    2.3.8 --> 6.5
    2.4.8 --> 6.5
    3.7 --> 6.2
    3.7 --> 6.5
    3.8 --> 6.3
    4.6 --> 6.3
    5.7 --> 6.6
    6.2 --> 6.7
    6.3 --> 6.7
    6.5 --> 6.6
    6.6 --> 6.7
    6.7 --> 6.8

    classDef research fill:#d4e6ff,stroke:#3366cc,stroke-width:2px
    classDef core fill:#d4f7d4,stroke:#2d862d,stroke-width:2px
    classDef model fill:#e6f7e6,stroke:#45a045,stroke-width:2px
    classDef security fill:#f0f7e6,stroke:#8cb84d,stroke-width:2px
    classDef storage fill:#e6f7f0,stroke:#45a08c,stroke-width:2px
    classDef infra fill:#fff2cc,stroke:#e6ac00,stroke-width:2px
    classDef fl fill:#e6e6ff,stroke:#6666ff,stroke-width:2px
    classDef ui fill:#ffe6f2,stroke:#cc66a3,stroke-width:2px
    classDef qa fill:#f2e6d9,stroke:#b38c5c,stroke-width:2px
```

These activities are cleanly divided into two graphs.

The Critical Path for the first and bigger graph is:

**6.5 --> 6.6 --> 6.7 --> 6.8**

This path has an estimated total duration of 11 weeks.

The Critical Path for the second graph is the only path:

**6.1 --> 6.4**

This path has an estimated total duration of 3 weeks.

### Full Diagram

```mermaid
graph TD
    %% Research & Design - Blue
    1.1:::research
    1.2:::research
    1.3:::research
    1.4:::research
    1.5:::research
    1.6:::research
    1.7:::research
    
    %% Core Framework Development - Green
    2.1.1:::core
    2.1.2:::core
    2.1.3:::core
    2.1.4:::core
    2.1.5:::core
    2.1.6:::core
    2.1.7:::core
    2.1.8:::core
    2.1.9:::core
    
    2.2.1:::model
    2.2.2:::model
    2.2.3:::model
    2.2.4:::model
    2.2.5:::model
    2.2.6:::model
    2.2.7:::model
    2.2.8:::model
    2.2.9:::model
    
    2.3.1:::security
    2.3.2:::security
    2.3.3:::security
    2.3.4:::security
    2.3.5:::security
    2.3.6:::security
    2.3.7:::security
    2.3.8:::security
    
    2.4.1:::storage
    2.4.2:::storage
    2.4.3:::storage
    2.4.4:::storage
    2.4.5:::storage
    2.4.6:::storage
    2.4.7:::storage
    2.4.8:::storage
    
    %% Infrastructure & Deployment - Orange
    3.1:::infra
    3.2:::infra
    3.3:::infra
    3.4:::infra
    3.5:::infra
    3.6:::infra
    3.7:::infra
    3.8:::infra
    
    %% Federated Learning Integration - Purple
    4.1:::fl
    4.2:::fl
    4.3:::fl
    4.4:::fl
    4.5:::fl
    4.6:::fl
    
    %% User Interface & Experience - Pink
    5.1:::ui
    5.2:::ui
    5.3:::ui
    5.4:::ui
    5.5:::ui
    5.6:::ui
    5.7:::ui
    
    %% Quality Assurance & Documentation - Brown
    6.1:::qa
    6.2:::qa
    6.3:::qa
    6.4:::qa
    6.5:::qa
    6.6:::qa
    6.7:::qa
    6.8:::qa

    %% Dependencies

    %%% Research & Design Dependencies
    1.1 --> 1.2
    1.2 --> 1.3
    1.2 --> 1.4
    1.2 --> 1.5
    1.3 --> 1.6
    1.4 --> 1.6
    1.5 --> 1.6
    1.6 --> 1.7
    
    %%% Quality Assurance Dependencies
    1.7 --> 6.1
    6.1 --> 6.4
    
    %%% Core Framework Dependencies
    6.4 --> 2.1.1
    6.4 --> 2.1.2
    6.4 --> 2.1.5
    6.4 --> 2.1.6
    6.4 --> 2.2.1
    6.4 --> 2.3.2
    6.4 --> 3.1
    6.4 --> 3.6
    
    2.1.1 --> 2.1.3
    2.1.1 --> 2.1.4
    2.1.1 --> 2.3.1
    2.1.1 --> 2.3.4
    2.1.2 --> 2.1.9
    2.1.3 --> 2.1.7
    2.1.3 --> 2.4.2
    2.1.3 --> 5.3
    2.1.4 --> 2.1.8
    2.1.4 --> 2.3.5
    2.1.4 --> 4.5
    2.1.4 --> 5.1
    2.1.5 --> 2.1.9
    2.1.5 --> 2.3.6
    2.1.5 --> 4.1
    2.1.6 --> 2.1.8
    2.1.6 --> 4.2
    2.1.7 --> 2.1.9
    2.1.7 --> 5.1
    2.1.7 --> 5.2
    2.1.8 --> 2.1.9
    2.1.8 --> 2.4.6
    2.1.8 --> 4.4
    2.1.8 --> 5.5
    
    %%% Model Definition Dependencies
    2.2.1 --> 2.2.2
    2.2.1 --> 2.2.3
    2.2.1 --> 2.2.6
    2.2.2 --> 2.2.4
    2.2.2 --> 5.2
    2.2.3 --> 2.2.4
    2.2.4 --> 2.2.5
    2.2.4 --> 2.2.7
    2.2.5 --> 2.2.9
    2.2.6 --> 2.2.7
    2.2.6 --> 2.2.8
    2.2.7 --> 2.2.9
    2.2.7 --> 2.4.1
    2.2.7 --> 2.4.4
    2.2.7 --> 4.2
    2.2.8 --> 2.2.9
    2.2.8 --> 2.4.4
    
    %%% Federation Management Dependencies
    2.3.1 --> 2.3.8
    2.3.2 --> 2.3.3
    2.3.2 --> 2.3.4
    2.3.2 --> 2.3.5
    2.3.3 --> 2.3.8
    2.3.4 --> 2.3.8
    2.3.4 --> 5.4
    2.3.5 --> 2.3.7
    2.3.5 --> 4.3
    2.3.6 --> 2.3.7
    2.3.6 --> 4.1
    2.3.7 --> 2.3.8
    
    %%% Model Storage Dependencies
    2.4.1 --> 2.4.2
    2.4.1 --> 2.4.3
    2.4.1 --> 2.4.5
    2.4.2 --> 2.4.8
    2.4.3 --> 2.4.8
    2.4.4 --> 2.4.6
    2.4.5 --> 2.4.7
    2.4.6 --> 2.4.8
    2.4.7 --> 2.4.8
    
    %%% Infrastructure Dependencies
    3.1 --> 3.2
    3.2 --> 3.3
    3.3 --> 3.4
    3.3 --> 3.5
    3.4 --> 3.7
    3.5 --> 3.7
    3.6 --> 3.7
    3.7 --> 3.8
    3.7 --> 6.2
    3.7 --> 6.5
    3.8 --> 6.3
    
    %%% Federated Learning Dependencies
    4.1 --> 4.3
    4.2 --> 4.3
    4.3 --> 4.4
    4.4 --> 4.5
    4.5 --> 4.6
    4.6 --> 6.3
    
    %%% UI/UX Dependencies
    5.1 --> 5.3
    5.1 --> 5.4
    5.1 --> 5.5
    5.2 --> 5.3
    5.2 --> 5.4
    5.2 --> 5.5
    5.3 --> 5.6
    5.4 --> 5.6
    5.5 --> 5.6
    5.6 --> 5.7
    
    %%% Final QA Dependencies
    2.1.9 --> 6.5
    2.2.9 --> 6.5
    2.3.8 --> 6.2
    2.3.8 --> 6.5
    2.4.8 --> 6.5
    5.7 --> 6.6
    6.2 --> 6.7
    6.3 --> 6.7
    6.5 --> 6.6
    6.6 --> 6.7
    6.7 --> 6.8

    classDef research fill:#d4e6ff,stroke:#3366cc,stroke-width:2px
    classDef core fill:#d4f7d4,stroke:#2d862d,stroke-width:2px
    classDef model fill:#e6f7e6,stroke:#45a045,stroke-width:2px
    classDef security fill:#f0f7e6,stroke:#8cb84d,stroke-width:2px
    classDef storage fill:#e6f7f0,stroke:#45a08c,stroke-width:2px
    classDef infra fill:#fff2cc,stroke:#e6ac00,stroke-width:2px
    classDef fl fill:#e6e6ff,stroke:#6666ff,stroke-width:2px
    classDef ui fill:#ffe6f2,stroke:#cc66a3,stroke-width:2px
    classDef qa fill:#f2e6d9,stroke:#b38c5c,stroke-width:2px
```

The full project critical path is:

**1.1 --> 1.2 --> 1.4 --> 1.6 --> 1.7 --> 6.1 --> 6.4 --> 2.2.1 --> 2.2.3 --> 2.2.4 --> 2.2.7 --> 2.4.1 --> 2.4.5 --> 2.4.7 --> 2.4.8 --> 6.5 --> 6.6 --> 6.7 --> 6.8**

This path has an estimated total duration of 54 weeks.

## Estimated Start & Finish

The following table shows the estimated Early/Late Start/Finish and the consequent slack available for each activity:

| ID | Early Start | Early Finish | Late Start | Late Finish | Slack |
|----|-------------|--------------|------------|-------------|-------|
| 1.1 | 1 | 3 | 1 | 3 | 0 |
| 1.2 | 4 | 5 | 4 | 5 | 0 |
| 1.3 | 6 | 7 | 7 | 8 | 1 |
| 1.4 | 6 | 8 | 6 | 8 | 0 |
| 1.5 | 6 | 7 | 7 | 8 | 1 |
| 1.6 | 9 | 9 | 9 | 9 | 0 |
| 1.7 | 10 | 10 | 10 | 10 | 0 |
| 2.1.1 | 14 | 17 | 20 | 23 | 6 |
| 2.1.2 | 14 | 16 | 39 | 41 | 25 |
| 2.1.3 | 18 | 22 | 24 | 28 | 6 |
| 2.1.4 | 18 | 24 | 34 | 38 | 16 |
| 2.1.5 | 14 | 17 | 30 | 33 | 16 |
| 2.1.6 | 14 | 18 | 27 | 31 | 13 |
| 2.1.7 | 23 | 28 | 29 | 34 | 6 |
| 2.1.8 | 24 | 27 | 34 | 37 | 10 |
| 2.1.9 | 29 | 31 | 42 | 44 | 13 |
| 2.2.1 | 14 | 16 | 14 | 16 | 0 |
| 2.2.2 | 17 | 19 | 18 | 20 | 1 |
| 2.2.3 | 17 | 20 | 17 | 20 | 0 |
| 2.2.4 | 21 | 23 | 21 | 23 | 0 |
| 2.2.5 | 24 | 27 | 39 | 42 | 15 |
| 2.2.6 | 17 | 18 | 22 | 23 | 5 |
| 2.2.7 | 24 | 27 | 24 | 27 | 0 |
| 2.2.8 | 19 | 21 | 29 | 31 | 10 |
| 2.2.9 | 28 | 29 | 43 | 44 | 15 |
| 2.3.1 | 18 | 20 | 40 | 42 | 22 |
| 2.3.2 | 14 | 17 | 31 | 34 | 17 |
| 2.3.3 | 18 | 19 | 41 | 42 | 23 |
| 2.3.4 | 18 | 22 | 37 | 41 | 19 |
| 2.3.5 | 24 | 27 | 35 | 38 | 11 |
| 2.3.6 | 18 | 24 | 34 | 38 | 16 |
| 2.3.7 | 28 | 31 | 39 | 42 | 11 |
| 2.3.8 | 32 | 33 | 43 | 44 | 11 |
| 2.4.1 | 28 | 31 | 28 | 31 | 0 |
| 2.4.2 | 32 | 34 | 39 | 41 | 7 |
| 2.4.3 | 32 | 34 | 39 | 41 | 7 |
| 2.4.4 | 28 | 33 | 32 | 37 | 4 |
| 2.4.5 | 32 | 36 | 32 | 36 | 0 |
| 2.4.6 | 34 | 37 | 38 | 41 | 4 |
| 2.4.7 | 37 | 41 | 37 | 41 | 0 |
| 2.4.8 | 42 | 44 | 42 | 44 | 0 |
| 3.1 | 14 | 15 | 31 | 32 | 17 |
| 3.2 | 16 | 18 | 33 | 35 | 17 |
| 3.3 | 19 | 22 | 36 | 39 | 17 |
| 3.4 | 23 | 25 | 40 | 42 | 17 |
| 3.5 | 23 | 24 | 41 | 42 | 18 |
| 3.6 | 14 | 14 | 42 | 42 | 28 |
| 3.7 | 26 | 27 | 43 | 44 | 17 |
| 3.8 | 28 | 30 | 46 | 48 | 18 |
| 4.1 | 25 | 28 | 31 | 34 | 6 |
| 4.2 | 28 | 30 | 32 | 34 | 4 |
| 4.3 | 31 | 35 | 35 | 39 | 4 |
| 4.4 | 36 | 37 | 40 | 41 | 4 |
| 4.5 | 38 | 41 | 42 | 45 | 4 |
| 4.6 | 42 | 44 | 46 | 48 | 4 |
| 5.1 | 29 | 34 | 35 | 40 | 6 |
| 5.2 | 29 | 33 | 36 | 40 | 7 |
| 5.3 | 35 | 37 | 41 | 43 | 6 |
| 5.4 | 35 | 36 | 42 | 43 | 7 |
| 5.5 | 35 | 36 | 42 | 43 | 7 |
| 5.6 | 38 | 39 | 44 | 45 | 6 |
| 5.7 | 40 | 42 | 46 | 48 | 6 |
| 6.1 | 11 | 12 | 11 | 12 | 0 |
| 6.2 | 34 | 37 | 48 | 51 | 14 |
| 6.3 | 45 | 47 | 49 | 51 | 4 |
| 6.4 | 13 | 13 | 13 | 13 | 0 |
| 6.5 | 45 | 48 | 45 | 48 | 0 |
| 6.6 | 49 | 51 | 49 | 51 | 0 |
| 6.7 | 52 | 53 | 52 | 53 | 0 |
| 6.8 | 54 | 54 | 54 | 54 | 0 |

## Gantt

To show a temporal schedule of the project a gantt chart is compiled:

```mermaid
gantt
    title Full Project Gantt Chart
    dateFormat  YYYY-MM-DD
    axisFormat  %d-%b-%Y
    %% Project start: 15 November 2025
    %% Each week = 7 days

    section Research
    1.1 :2025-11-15, 2025-12-05
    1.2 :2025-12-06, 2025-12-19
    1.3 :2025-12-20, 2026-01-02
    1.4 :2025-12-20, 2026-01-09
    1.5 :2025-12-20, 2026-01-02
    1.6 :2026-01-17, 2026-01-23
    1.7 :2026-01-24, 2026-01-30

    section Core
    2.1.1 :2026-02-21, 2026-03-20
    2.1.2 :2026-02-21, 2026-03-06
    2.1.3 :2026-03-14, 2026-04-17
    2.1.4 :2026-03-14, 2026-04-25
    2.1.5 :2026-02-21, 2026-03-20
    2.1.6 :2026-02-21, 2026-03-27
    2.1.7 :2026-04-18, 2026-05-23
    2.1.8 :2026-04-25, 2026-05-16
    2.1.9 :2026-05-24, 2026-06-07

    section Model
    2.2.1 :2026-02-21, 2026-03-06
    2.2.2 :2026-03-07, 2026-03-21
    2.2.3 :2026-03-07, 2026-03-28
    2.2.4 :2026-03-29, 2026-04-11
    2.2.5 :2026-04-12, 2026-05-09
    2.2.6 :2026-03-07, 2026-03-14
    2.2.7 :2026-04-12, 2026-05-09
    2.2.8 :2026-03-14, 2026-03-28
    2.2.9 :2026-05-10, 2026-05-17

    section Federation
    2.3.1 :2026-03-14, 2026-03-28
    2.3.2 :2026-02-21, 2026-03-20
    2.3.3 :2026-03-21, 2026-03-28
    2.3.4 :2026-03-14, 2026-04-17
    2.3.5 :2026-04-12, 2026-05-09
    2.3.6 :2026-03-14, 2026-04-25
    2.3.7 :2026-05-10, 2026-05-31
    2.3.8 :2026-06-14, 2026-06-21

    section Storage
    2.4.1 :2026-05-10, 2026-05-31
    2.4.2 :2026-06-14, 2026-06-28
    2.4.3 :2026-06-14, 2026-06-28
    2.4.4 :2026-05-10, 2026-06-14
    2.4.5 :2026-06-14, 2026-07-19
    2.4.6 :2026-06-28, 2026-07-19
    2.4.7 :2026-07-19, 2026-08-23
    2.4.8 :2026-09-06, 2026-09-20

    section Infrastructure
    3.1 :2026-02-21, 2026-02-28
    3.2 :2026-03-07, 2026-03-21
    3.3 :2026-03-22, 2026-04-18
    3.4 :2026-04-19, 2026-05-09
    3.5 :2026-04-19, 2026-05-02
    3.6 :2026-02-21, 2026-02-21
    3.7 :2026-05-10, 2026-05-24
    3.8 :2026-05-25, 2026-06-14

    section FL
    4.1 :2026-05-02, 2026-05-30
    4.2 :2026-05-30, 2026-06-13
    4.3 :2026-06-14, 2026-07-19
    4.4 :2026-07-26, 2026-08-02
    4.5 :2026-08-09, 2026-09-06
    4.6 :2026-09-20, 2026-10-04

    section UI
    5.1 :2026-06-01, 2026-07-06
    5.2 :2026-06-01, 2026-06-29
    5.3 :2026-07-13, 2026-07-27
    5.4 :2026-07-13, 2026-07-20
    5.5 :2026-07-13, 2026-07-20
    5.6 :2026-07-27, 2026-08-03
    5.7 :2026-08-10, 2026-08-24

    section QA & Doc
    6.1 :2026-01-31, 2026-02-14
    6.2 :2026-07-19, 2026-08-09
    6.3 :2026-09-14, 2026-09-28
    6.4 :2026-02-15, 2026-02-15
    6.5 :2026-09-14, 2026-10-05
    6.6 :2026-10-12, 2026-10-26
    6.7 :2026-10-27, 2026-11-10
    6.8 :2026-11-17, 2026-11-17
```

## Project Proposal

### Executive Summary

### Background

### Objective

### Overview of Approach

### Detailed Statements of Work

### Risk Analysis

### Time and Cost Summary

