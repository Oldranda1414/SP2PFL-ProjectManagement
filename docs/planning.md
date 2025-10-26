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

### Research & Design

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 1.1 | Study and interpret the Secure Average Computation algorithm (Wink et al., 2021) |
| 1.2 | Define system requirements and success metrics |
| 1.3 | Design federated architecture (server–peer topology, communication flow) |
| 1.4 | Define security and encryption mechanisms for peer communication |
| 1.5 | Define API specifications and endpoints | 1.1.3.1
| 1.6 | Design data schema and metadata format for federated datasets |
| 1.7 | Produce software architecture documentation and design diagrams |
| 1.8 | Validate design through technical review |

### Core Framework Development

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 2.1 | Implement peer registration and authentication subsystem |
| 2.2 | Implement role and permission management |
| 2.3 | Implement federated orchestration service (task coordination, scheduling) |
| 2.4 | Develop Secure Average Computation module |
| 2.5 | Implement communication protocol for distributed training |
| 2.6 | Develop API endpoints for peer and admin operations | 1.1.3.1
| 2.7 | Integrate monitoring and logging capabilities |
| 2.8 | Conduct unit and integration testing for core modules |

### Infrastructure & Deployment

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 3.1 | Configure development and testing environments |
| 3.2 | Implement containerization (e.g., Docker) for peer and server components | 1.1.2.2
| 3.3 | Set up orchestration (Kubernetes or similar) | 1.1.2.2
| 3.4 | Create CI/CD pipelines for automated builds and deployment |
| 3.5 | Configure cloud infrastructure for distributed experiments |
| 3.6 | Establish data privacy and network security policies |
| 3.7 | Deploy framework to production (SAAS hosting) |
| 3.8 | Conduct scalability and performance tests |

### Federated Learning Integration

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 4.1 | Implement model aggregation logic using Secure Average Computation |
| 4.2 | Define model update serialization and exchange protocol |
| 4.3 | Handle asynchronous peer updates and dropout resilience |
| 4.4 | Implement audit trail and logging of training rounds |
| 4.5 | Integrate algorithm with orchestration and monitoring services |
| 4.6 | Validate model performance and convergence under federation |

### User Interface & Experience

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 5.1 | Design admin dashboard (federation overview, peer management) | 1.1.1.2
| 5.2 | Design peer organization dashboard (local training, participation status) |
| 5.3 | Implement role-based access controls in the UI |
| 5.4 | Integrate credential management and registration flows |
| 5.5 | Add notifications for federation events and status updates |
| 5.6 | Conduct usability testing and collect feedback |
| 5.7 | Implement help, documentation, and onboarding pages |

### Quality Assurance & Documentation

| ID | Activity | Related User Stories |
|----|----------|----------------------|
| 6.1 | Develop comprehensive test plan (unit, integration, system, acceptance) |
| 6.2 | Perform security and compliance testing |
| 6.3 | Conduct performance benchmarking |
| 6.4 | Maintain traceability between user stories and test cases |
| 6.5 | Prepare technical documentation (API docs, deployment guide) |
| 6.6 | Write user documentation and quick-start manuals |
| 6.7 | Conduct final validation and acceptance testing |
| 6.8 | Prepare lessons learned and project closure report |

