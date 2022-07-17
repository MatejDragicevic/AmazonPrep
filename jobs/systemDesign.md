# System Design
sytem design part from
[interview prep](https://www.amazon.jobs/en/software-development-interview-prep?INTCMPID=OAAJAZ100028B#/)
- good design leads to extensible, bugfree, long-lived code
- scalable and maintainable
- OO best practices
- think about:
    - software components
    - distributed systems
    - system trade-offs
## SD assessment
- black box design a software system
- deliver with considering:
    - deployment
    - scaling
    - failures
    - availability
    - performance
- discuss latency and concurrency
## how to prepare topics
- software systems:
    - software components
    - data storage
    - business logic to make decisions
    - api
    - process
- knowledge:
    - distributed systems
    - Service Oriented Architecture(SOA)
    - n-tiered Soft. Arch.
- draw it by hand

## How to showcase your system design
criteria and pro tips for addressing your skills

### Asking clarifying questions
scope-down and define requirements

- interviewer is there to help you with
    - clarifying questions
    - assumptions
    - providing customer perspective
    - start with customer and work back
        - who and why?
        - functionality expectations?
        - customer assumptions that should be there(fast, secure)
        - how to tackle big growth? how does it influence design?
- what problems is the systems solving?
- interviewer as a customer
- intentionally vague requirements with clarifications
- write/raise requirements and assumptions and base design on them
- feel free to create a diagram to clarify

### fulfilling requirements
design system that fulfills requirements
(constraints, scalability, maintenance)

- influences are typicall:
    - non-functional requirements
        - amount of load
        - load distribution
        - security
    - ways of interacting with the system
        - user access
        - scheduled processes
        - syncrhonous/asynchronous communication)
        - data flow
- always mention assumptions
- spend majority of time on critical requirements and core functionality
- justify design choices
- design the solution for scale(more transactions work?)
- research and read through best practices in the tech stack or infrastructure
- know how code and hardware can be maintained, scaled and made available
### desinging for performance
design for operational performance
and plans for failure
and measure the results(metrics)
- when the design solves the problem, think of operations
- think operations and resilience in your design
- questions:
    - key business and technical metrics for the system?
    - how to identify problems?
    - bottlenecks and pain points?
    - failure points?
    - redundancy to build to reduce single points of failure?
    - get logs and debug?
### identify shortcomings
shortcomings and tradeoffs with different designs
(performance, fault, tolerance, dependencies)
- describe if there are multiple designs that satisfy the requirements
- describe the trade-offs, choose and explain why
- explain your thought process
- know how to deep dive into areas of the design

## Othere important system considerations
- SCALING IS CRITICAL AT AMAZON
    - caching
    - load balancing
    - non-relational databases
    - micro services
    - sharding
- fault tolerance translate to the customer obsession LP
    - if dependencies are failing, still serve the customer
    - frugal redundancy is paramount to success
