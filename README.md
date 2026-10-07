# Complete Placement Topic List: SDE / Fresher Interviews (India)

Full-coverage topic list for **OOP (C++), DBMS, SQL, Operating Systems, Computer Networks, System Design**, plus the non-technical areas every placement process tests.

---

## Tier Legend

Not every topic carries equal weight. Use the tiers to decide what to study first.

| Tier | Meaning |
|------|---------|
| **A** | Asked constantly. Study first. |
| **B** | Common follow-ups, or asked at many companies. |
| **C** | Rare or deep. Needed only for completeness. |

> **Time estimate:** A + B + C is roughly **250-350 hours**. A + B alone covers almost every fresher interview.

---

## How to Use This File

1. **Pass 1:** Study only **A** topics, subject by subject.
2. **Pass 2:** Add **B** topics.
3. **Pass 3:** Touch **C** topics only if time remains.
4. Use **one resource per subject**. Don't mix sources.
5. After each topic, close everything and explain it aloud. Keep a 1-2 page cheat sheet per subject (comparison tables, one-line definitions, your own mistakes, diagrams).

**Suggested order:** OOP → DBMS + SQL → OS → CN → LLD → HLD

---

## Table of Contents

1. [OOP in C++](#1-oop-in-c)
2. [DBMS](#2-dbms)
3. [SQL](#3-sql)
4. [Operating Systems](#4-operating-systems)
5. [Computer Networks](#5-computer-networks)
6. [System Design](#6-system-design)
7. [Everything Else a Placement Tests](#7-everything-else-a-placement-actually-tests)

---

## 1. OOP in C++

| Area | Topics | Tier |
|------|--------|------|
| Foundations | Procedural vs OOP, class/object, struct vs class, access specifiers, member functions, scope resolution `::`, `this`, static data/functions, `const` members and `const` objects, `mutable`, inline functions, namespaces | A |
| Memory basics | Stack vs heap, `new`/`delete` vs `malloc`/`free`, memory leak, dangling pointer, pointers vs references, `nullptr` | A |
| Constructors / destructors | Default, parameterized, copy, move, delegating, `explicit`, initializer list, destructor, call order, private constructor, `= default` / `= delete` | A |
| Four pillars | Encapsulation, abstraction, inheritance, polymorphism | A |
| Inheritance | Types, public/protected/private modes, ctor/dtor order, function hiding, multiple inheritance, diamond problem, virtual inheritance, `final`, `override` | A |
| Compile-time polymorphism | Function overloading, operator overloading, templates | A/B |
| Runtime polymorphism | Virtual functions, vtable/vptr, late vs early binding, pure virtual, abstract class, interface, virtual destructor, object slicing, covariant return types | A |
| Virtual edge cases | Virtual calls inside ctor/dtor, virtual constructor (why not), virtual static (why not), default arguments with virtual, pure virtual with a body | B |
| Copy and ownership | Shallow vs deep copy, copy assignment, self-assignment check, Rule of 0/3/5, copy elision | A |
| Modern C++ | rvalue references, move constructor/assignment, `std::move`, `std::forward`, RAII, `unique_ptr`/`shared_ptr`/`weak_ptr`, circular reference, `auto`, lambdas, `noexcept` | B (`std::forward` = C) |
| Operator overloading | Rules, non-overloadable operators, unary/binary, `<<` / `>>`, `==`, `[]`, `()`, pre/post `++`, member vs friend, conversion operators | B |
| Friend | Friend function/class | B |
| Relationships | Association, aggregation, composition, dependency, IS-A vs HAS-A, composition over inheritance | A |
| Templates | Function and class templates, specialization, STL as generic design | B/C |
| Exceptions | `try`/`catch`/`throw`, exceptions in ctor/dtor, RAII for cleanup, exception safety | B |
| Casting / RTTI | `static_cast`, `dynamic_cast`, `const_cast`, `reinterpret_cast`, `typeid`, C-style cast | B |
| Misc | Function pointers, functors, pointer-to-member, `volatile`, enums (`enum class`), C vs C++, C++ vs Java/Python OOP differences | B/C |

---

## 2. DBMS

| Area | Topics | Tier |
|------|--------|------|
| Basics | File system vs DBMS, DBMS vs RDBMS, 3-schema architecture, data independence, DDL/DML/DCL/TCL/DQL, schema vs instance | A/B |
| ER model | Entities, attribute types, relationships, cardinality, participation, weak entity, specialization/generalization/aggregation, ER → tables | B |
| Keys / constraints | Super, candidate, primary, alternate, foreign, composite, surrogate, unique, NOT NULL, CHECK, DEFAULT, referential integrity, ON DELETE CASCADE | A |
| Relational algebra | Select, project, union, difference, cross product, joins, division | C |
| Normalization | Anomalies (insert/update/delete), functional dependency, attribute closure, finding candidate keys, 1NF, 2NF, 3NF, BCNF, lossless join, dependency preservation, denormalization | A |
| Advanced normal forms | MVD, 4NF, 5NF, Armstrong axioms, canonical cover | C |
| Transactions | ACID, states, schedules, concurrency problems, isolation levels, commit/rollback/savepoint | A |
| Concurrency control | Shared/exclusive locks, 2PL, strict 2PL, deadlock handling (wait-die, wound-wait, wait-for graph), optimistic vs pessimistic, MVCC | B |
| Serializability / recovery | Conflict/view serializability, recoverable/cascadeless/strict schedules, timestamp ordering, WAL, checkpoints, undo/redo, ARIES, shadow paging | B (recovery math = C) |
| Indexing | Clustered/non-clustered, dense/sparse, B-tree vs B+ tree, hash index, composite index, covering index, selectivity, when indexes hurt | A |
| Query processing | Execution plan, EXPLAIN, join algorithms (nested loop/hash/merge), SARGable queries, N+1 problem, pagination | B |
| DB objects | Views, materialized views, stored procedures vs functions, triggers, cursors, sequences/auto-increment, temp tables | B |
| Scaling / NoSQL | Replication, partitioning, sharding, CAP, BASE, eventual consistency, NoSQL types (document/key-value/column/graph), SQL vs NoSQL, OLTP vs OLAP, data warehouse, ETL | A/B |
| Security | SQL injection, prepared statements, GRANT/REVOKE, roles, encryption | B |
| Standard comparisons | DELETE/TRUNCATE/DROP, WHERE/HAVING, UNION/UNION ALL, primary vs unique, view vs table, CHAR vs VARCHAR, procedure vs function, trigger vs procedure | A |

---

## 3. SQL

| Area | Topics | Tier |
|------|--------|------|
| Basics | SELECT, WHERE, ORDER BY, LIMIT/OFFSET/TOP, aliases, DISTINCT, LIKE/wildcards, IN, BETWEEN, `IS NULL`, operators | A |
| Aggregation | COUNT/SUM/AVG/MIN/MAX, GROUP BY, HAVING, logical order of execution, `COUNT(*)` vs `COUNT(col)` | A |
| Joins | INNER, LEFT, RIGHT, FULL, CROSS, SELF, natural join, semi/anti join | A |
| Set operations | UNION, UNION ALL, INTERSECT, EXCEPT/MINUS | A |
| Subqueries | Scalar, row, table, correlated, in FROM/SELECT/WHERE, EXISTS/NOT EXISTS, ANY/ALL | A |
| Conditional / NULL | CASE, COALESCE, NULLIF, IFNULL, three-valued logic | A |
| Functions | String, date/time, numeric, type casting | B |
| DDL / DML | CREATE/ALTER/DROP, constraints, INSERT/UPDATE/DELETE, INSERT…SELECT, UPSERT/MERGE, transactions in SQL | A/B |
| CTEs | Basic CTE, recursive CTE | B / C |
| Window functions | ROW_NUMBER, RANK, DENSE_RANK, NTILE, LAG, LEAD, FIRST/LAST_VALUE, `SUM() OVER`, PARTITION BY, frames, moving average | A/B |
| Pivoting | Conditional aggregation, PIVOT/UNPIVOT | B/C |
| Performance | Index usage in queries, avoiding `SELECT *`, SARGable predicates, reading EXPLAIN | B |
| Classic problems | Nth highest salary, second highest without LIMIT, duplicates (find/delete), top N per department, employees earning more than manager, customers with no orders, consecutive numbers/days, running total, median, gaps and islands, swap values, missing IDs, month-over-month change, active-user/retention, rows-to-columns | A/B |
| Dialect awareness | MySQL vs PostgreSQL vs SQL Server vs Oracle syntax differences | B |

---

## 4. Operating Systems

| Area | Topics | Tier |
|------|--------|------|
| Intro | OS goals/functions, OS types (batch, multiprogramming, time-sharing, real-time, distributed), kernel types (monolithic/micro/hybrid), system calls, user vs kernel mode, interrupts vs traps, shell, boot process | A/B |
| Processes | Program vs process, memory layout (text/data/heap/stack), states, PCB, context switch, `fork`/`exec`/`wait`/`exit`, zombie, orphan, daemon | A |
| Threads | Process vs thread, user vs kernel threads, multithreading models, thread pool, thread safety, concurrency vs parallelism | A |
| Scheduling | Criteria, preemptive vs non-preemptive, FCFS, SJF, SRTF, RR, priority, multilevel queue, MLFQ, HRRN, convoy effect, starvation and aging, real-time (RMS/EDF), Linux CFS | A (HRRN/RMS/EDF/CFS = C) |
| Synchronization | Race condition, critical section and its 3 requirements, Peterson's, TSL/CAS, mutex, spinlock, semaphores, monitors, condition variables, producer-consumer, readers-writers, dining philosophers, sleeping barber, priority inversion, livelock | A/B |
| Deadlock | 4 conditions, resource allocation graph, prevention, avoidance (safe state, Banker's), detection, recovery, ostrich algorithm, deadlock vs starvation vs livelock | A |
| Memory management | Logical vs physical address, MMU, contiguous allocation (first/best/worst fit), internal/external fragmentation, compaction, swapping | A |
| Paging / segmentation | Page table, multi-level paging, inverted page table, TLB, effective access time, segmentation, segmentation with paging | A/B |
| Virtual memory | Demand paging, page fault handling, page replacement (FIFO, Optimal, LRU, Clock, LFU), Belady's anomaly, frame allocation, thrashing, working set, copy-on-write, memory-mapped files | A/B |
| Memory hierarchy | Cache levels, locality of reference, hit/miss ratio, buddy and slab allocators | B/C |
| IPC | Pipes, named pipes, message queues, shared memory, sockets, signals | B |
| File systems | File attributes, access methods, directory structure, allocation (contiguous/linked/indexed), inode, free-space management, hard vs soft links, journaling, FAT/NTFS/ext4 | B/C |
| I/O and disk | Polling vs interrupts vs DMA, buffering/spooling, drivers, disk scheduling (FCFS/SSTF/SCAN/C-SCAN/LOOK), RAID, HDD vs SSD | B/C |
| Virtualization | VMs vs containers, hypervisor types, Docker basics | B |
| Security | Protection domains, authentication, access control | C |
| Linux practical | `ls`, `grep`, `chmod`, `ps`, `top`, `kill`, pipes and redirection, permissions | B |

---

## 5. Computer Networks

| Area | Topics | Tier |
|------|--------|------|
| Basics | LAN/WAN/MAN/PAN, topologies, devices (hub, switch, bridge, router, gateway, modem, AP), media, bandwidth/latency/throughput, delay types, packet vs circuit switching, client-server vs P2P | A/B |
| Models | OSI, TCP/IP, encapsulation, PDUs, protocol-per-layer map | A |
| Data link | Framing, error detection (parity/checksum/CRC), Hamming code, flow control (stop-and-wait/GBN/SR), ALOHA, CSMA/CD, CSMA/CA, Ethernet, MAC, switching and learning, VLAN, STP, collision vs broadcast domain | B/C |
| Network layer | IPv4, classes, CIDR, subnetting, VLSM, private vs public IP, NAT/PAT, IPv6, ICMP (ping/traceroute), DHCP, ARP, fragmentation/MTU, TTL, IP header | A/B (subnetting math = C) |
| Routing | Static vs dynamic, distance vector (RIP), link state (OSPF), BGP, routing table, longest prefix match | B/C |
| Transport | Ports, sockets, multiplexing, TCP header, handshake, termination, sequence/ack, retransmission, sliding window, flow control, congestion control (slow start, avoidance, fast retransmit/recovery, Tahoe/Reno), TIME_WAIT, SYN flood, UDP, TCP vs UDP, QUIC | A/B |
| Socket programming | `socket`/`bind`/`listen`/`accept`/`connect`/`send`/`recv`, blocking vs non-blocking, `select`/`poll`/`epoll` | B |
| DNS | Hierarchy, recursive vs iterative, caching/TTL, record types (A/AAAA/CNAME/MX/NS/TXT) | A |
| HTTP | Versions (1.0/1.1/2/3), methods, headers, status codes, idempotency, persistent connections, caching headers, ETag, conditional GET, CORS | A |
| Web auth | Cookies, sessions, JWT, OAuth basics, Basic/Bearer/API-key auth | A/B |
| APIs / real-time | REST, GraphQL vs REST, gRPC, WebSockets, SSE, long polling, webhooks | A/B |
| Security | HTTPS/TLS handshake, certificates and CAs, symmetric vs asymmetric, digital signature, hashing, Diffie-Hellman, MITM, DDoS, XSS, CSRF, SQL injection | A/B |
| Other protocols | SMTP/POP3/IMAP, FTP/SFTP, SSH, Telnet, NTP | B/C |
| Infra | Proxy vs reverse proxy, load balancer (L4/L7, algorithms), CDN, firewall, VPN, API gateway, IDS | B |
| Tools | `ping`, `traceroute`, `nslookup`/`dig`, `netstat`, `curl`, `ipconfig`/`ifconfig` | B |
| Wireless | Wi-Fi basics, Bluetooth, cellular | C |
| Flagship question | "What happens when you type a URL in the browser?" | A |

---

## 6. System Design

### 6.1 Low-Level Design (LLD)

| Area | Topics | Tier |
|------|--------|------|
| Principles | OOP, SOLID, DRY/KISS/YAGNI, Law of Demeter, composition over inheritance, coupling/cohesion, dependency injection | A |
| Modeling | Requirement gathering, entities, relationships, UML (class, sequence, use-case, activity) | A/B |
| Creational patterns | Singleton, Factory Method, Abstract Factory, Builder, Prototype | A (Abstract Factory/Prototype = B) |
| Structural patterns | Adapter, Decorator, Facade, Proxy, Composite, Bridge, Flyweight | B (Flyweight = C) |
| Behavioral patterns | Strategy, Observer, State, Command, Template Method, Iterator, Chain of Responsibility, Mediator, Memento, Visitor | A (Strategy/Observer/State) / B / C (Visitor) |
| Practical concerns | Thread safety, extensibility, error handling | B |

**LLD practice problems**

| Tier | Problems |
|------|----------|
| A | Parking Lot, Library Management, Tic-Tac-Toe, LRU Cache |
| B | Vending Machine, ATM, Elevator, BookMyShow, Snake & Ladder, Logger, Splitwise, Food Ordering, Hotel Booking |
| C | Chess, LFU Cache, Pub-Sub, Task Scheduler, Rate Limiter, Notification Service, File System, Traffic Signal, Airline Reservation, Shopping Cart, Meeting Scheduler, Text Editor |

### 6.2 High-Level Design (HLD)

| Area | Topics | Tier |
|------|--------|------|
| Fundamentals | Functional vs non-functional requirements, scalability, availability, reliability, latency vs throughput, consistency, fault tolerance, SLA/SLO/SLI | A |
| Theory | CAP, PACELC, BASE, eventual consistency | B |
| Estimation | QPS, storage, bandwidth calculations | B |
| Load balancing | Algorithms, L4/L7, health checks | A |
| Caching | Cache types, cache-aside/write-through/write-back/write-around, eviction (LRU/LFU/TTL), invalidation, stampede, Redis/Memcached | A |
| CDN | Push vs pull, edge caching | B |
| Databases | SQL vs NoSQL, indexing, master-slave/multi-master replication, sharding strategies, consistent hashing, hot keys, denormalization | A/B |
| Messaging | Message queues, pub-sub, Kafka basics, async processing | B |
| Architecture | Monolith vs microservices, API gateway, service discovery, stateless vs stateful, sessions | B |
| API design | REST, pagination, versioning, idempotency, rate limiting, authN/authZ | A/B |
| Storage / search | Blob/object storage, inverted index/Elasticsearch basics | B |
| Building blocks | Unique ID generation (UUID/Snowflake), Bloom filters, heartbeats | B/C |
| Resilience | Circuit breaker, retries with backoff, graceful degradation | B |
| Observability | Monitoring, logging, tracing, alerting | B |
| Advanced distributed | Leader election, consensus (Paxos/Raft), 2PC, saga, CQRS, event sourcing, Zookeeper, geo-distribution | C |
| Infra | CI/CD basics, Docker, Kubernetes | B / C |

**HLD practice problems**

| Tier | Problems |
|------|----------|
| A | URL Shortener |
| B | Rate Limiter, Notification System, Chat App, Pastebin, News Feed |
| C | Twitter, Instagram, YouTube/Netflix, E-commerce, Food Delivery, Ride Sharing, Dropbox/Drive, Web Crawler, Typeahead, Distributed Cache, Key-Value Store, Payment System, Leaderboard/Top-K, Ticket Booking, Metrics System |

---

## 7. Everything Else a Placement Actually Tests

These sit outside the five core subjects, but they appear in nearly every placement process.

| Area | Topics | Tier |
|------|--------|------|
| Projects | Architecture, tech choices and why, DB/API design, challenges, improvements, metrics, what you'd do differently | A |
| HR / behavioral | Tell me about yourself, strengths/weaknesses, why this company, conflict, failure, leadership, 5-year plan, questions for the interviewer | A |
| Aptitude | Quant (percentages, ratios, time-work-speed, probability, P&C), logical reasoning, verbal ability | A for OA-heavy companies |
| Language equivalents | OOP and core concepts in Java and/or Python (some rounds don't allow C++) | A/B |
| Software engineering | SDLC, Agile/Scrum, testing types (unit/integration/regression), debugging approach | B |
| Git | commit/branch/merge/rebase/stash, merge conflicts, pull request flow | B |
| Web basics | HTML/CSS/JS, DOM manipulation, `fetch`/async-await | B for web-OA companies |
| Cloud basics | What AWS/Azure/GCP offer (compute, storage, DB, queues), serverless vs servers | B/C |
| Puzzles | Classic logic and probability puzzles | C |
| Resume hygiene | Working links, quantified bullet points, every line defensible | A |
