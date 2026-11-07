# System Design Portfolio

A learning portfolio covering **Low-Level Design (LLD)**, **High-Level Design (HLD)**, Linux systems, and network-software architecture.

The focus is on explaining requirements, interfaces, data flow, bottlenecks, failure handling, trade-offs, and how a design can be validated.

## Design documents

| Design | Area | Status |
|---|---|---|
| [High-Performance NAT Gateway](03-Networking-Design/NAT-Gateway.md) | Packet processing, session state, NAT | Initial design |
| [Network Firewall](03-Networking-Design/Network-Firewall.md) | Policy evaluation, stateful filtering | Initial design |
| [Load Balancer](02-High-Level-Design/Load-Balancer.md) | L4 traffic distribution, health checks | Initial design |
| [VPN Gateway](03-Networking-Design/VPN-Gateway.md) | IPsec / SSL VPN concepts | Initial design |

## Suggested document structure

Every design should cover:
1. Problem statement and scope
2. Functional requirements
3. Non-functional requirements and assumptions
4. Capacity estimates (with explicit assumptions)
5. High-level architecture and request / packet flow
6. Components, interfaces, and data models
7. Concurrency, scaling, and performance
8. Failure modes and recovery
9. Security and observability
10. Trade-offs, open questions, and validation plan

## Important engineering note

Capacity targets such as 10 million packets per second or one million concurrent sessions are **design goals**, not measured results. Real throughput depends on hardware, packet size, traffic mix, NIC queues, CPU, memory, configuration, and benchmark methodology. Do not claim a target is achieved until it is measured and documented.

## Diagram format

Architecture diagrams use Mermaid so GitHub can render them directly in Markdown. Supporting source code or experiments should be kept separate from conceptual design documents.

## Learning roadmap

- [x] NAT Gateway — initial architecture
- [x] Stateful Firewall — initial architecture
- [x] Load Balancer — initial architecture
- [x] VPN Gateway — initial architecture
- [ ] Add capacity calculations and sequence diagrams
- [ ] Add LLD class diagrams and interfaces
- [ ] Add reproducible performance test plans