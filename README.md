# CS 230 – Operating Platforms (Software Design Document)

This repository contains a portfolio artifact from **CS 230: Operating Platforms** at **Southern New Hampshire University (SNHU)**.

The artifact is a **Software Design Document** for the “Draw It or Lose It” project. It focuses on translating requirements into a platform-aware design that supports scalability, reliability, security, and cross-platform deployment considerations.

---

## Portfolio Artifact

- **Software Design Document (DOCX):** [CS_230_Project_Three_Software_Design.docx](docs/CS_230_Project_Three_Software_Design.docx)  
- **Software Design Document (PDF):** [CS_230_Project_Three_Software_Design.pdf](docs/CS_230_Project_Three_Software_Design.pdf)

> The PDF is best for quick viewing in-browser. The DOCX is included as the editable source.

---

## Project Summary (Client + Requirements)

**Client:** The Gaming Room  
**Product:** *Draw It or Lose It*  
**Goal:** Expand an existing game to support additional operating platforms while maintaining a smooth experience for concurrent users.

Key considerations addressed in the design:
- Cross-platform support and deployment strategy
- Scalability and concurrency for multiple players/sessions
- Storage and memory management decisions
- Security and distributed communication considerations
- Architectural choices that support maintainability and growth

---

## Reflection

### What I did particularly well
I organized the design around real constraints and requirements, tying recommendations directly to the client’s needs (platform selection, architecture approach, storage strategy, and security controls). My intent was to make the document usable as a blueprint for implementation and deployment decisions.

### How the design document helped guide development
Writing the design document clarified tradeoffs early—especially around scaling, session management, and storage. Documenting these decisions reduces ambiguity later and helps align implementation with real-world deployment constraints.

### What I would revise or improve
If I revisited this project, I would expand the **system architecture view** and include a simple diagram showing how major components interact (client → load balancing → application instances → data/storage services). A visual would make the relationships and data flow easier to understand at a glance.

### How I interpret user needs and turn them into design decisions
I start by identifying what “success” looks like for the user and then translate those needs into clear requirements. From there, I evaluate platform constraints and tradeoffs (performance, reliability, security, scalability) and choose designs that best support the requirements.

---

## Repository Structure

```text
.
├── README.md
└── docs/
    ├── CS_230_Project_Three_Software_Design.docx
    └── CS_230_Project_Three_Software_Design.pdf
