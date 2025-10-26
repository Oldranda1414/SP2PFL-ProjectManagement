Once the POS is approved, the Planning phase can start.

## Joint Project Planning Sessions

Joint Project Planning Sessions (JPPS) are scheduled. The entire development team and project manager will partecipate to these meetings.

The PM schedules and organizes the meetings deciding:

- Attendees: The entire development team (10 members), Finance Manager, Customer Experience Analyst and the PM himself
- Facilities: The meeting room in OpenML offices is spacious enough for the JPPS to take place
- Equipment: The meeting room provides a wide round table with enough seats for all attendees. Office laptops and pen and paper will be provided

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
- Project proposal

## Work Breakdown Structure

Activities are constructed to represent the work to be done to satisfy the requirements expressed by the user stories.

Since the relationship between user stories and activities is non trivial Requirements Traceability Matrixes (RTM) are used to highlight these relationships.

Since some activities are totally fully they do not have a user story related.

### Research & Design

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 1.1 | Study and interpret the Secure Average Computation algorithm (Wink et al., 2021) | 3.3.2.1 |
| 1.3 | Design federated architecture (server–peer topology, communication flow) | 3.3.1.2 |
| 1.4 | Define security and encryption mechanisms for peer communication | 3.2.1.1, 3.2.1.2, 3.2.1.3 |
| 1.5 | Define API specifications and endpoints | 1.1.3.1, 3.1.1.3, 3.1.3.2, 3.1.4.4, 3.3.1.6, 3.3.3.4, 4.2.1.1 |
| 1.6 | Design data schema and metadata format for federated datasets | 2.1.1.1, 2.1.1.2, 2.1.3.2 |
| 1.7 | Produce software architecture documentation and design diagrams | |
| 1.8 | Validate design through technical review | |

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

