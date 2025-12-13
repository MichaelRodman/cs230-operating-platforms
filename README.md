# CS 230 Operating Platforms – Draw It or Lose It Software Design Document

## Portfolio Artifact
- **Software Design Document (DOCX):** [CS 230 Project Three Software Design.docx](docs/CS%20230%20Project%20Three%20Software%20Design.docx)
- **Software Design Document (PDF):** [CS 230 Project Three Software Design.pdf](docs/CS%20230%20Project%20Three%20Software%20Design.pdf)

## Client and Requirements Summary
**The client** for this course was **The Gaming Room**, a company that wanted to expand their existing game, *Draw It or Lose It*, beyond Android to support additional operating platforms. The goal was to design a web-based architecture that could support multiple teams and players, manage game sessions reliably, and scale as usage increases. Key requirements included unique naming for games/teams, support for concurrent games, and a platform design that considers operating systems, memory and storage management, distributed systems/network communication, and security.

## What I Did Particularly Well
I did particularly well at organizing the design document in a way that directly ties technical decisions to the client’s needs. In the Recommendations section, I provided clear, actionable choices for operating platform, architecture, storage, memory management, distributed communication, and security controls, which makes the document usable as a blueprint for development and deployment.

## How the Design Document Helped When Developing Code
Working through the design document helped clarify constraints and decisions before implementation. By documenting platform choices, scaling strategy, and how game state and assets should be handled, it reduced uncertainty and helped ensure the code design aligns with real-world deployment needs (for example, avoiding storing large assets in memory and designing stateless services that can scale horizontally).

## What I Would Revise and How I Would Improve It
If I could revise one part of the document, I would expand the **System Architecture View** and include a simple diagram showing the n-tier layout (client → load balancer → application instances → database/cache → object storage/CDN). Adding a visual diagram would make the relationships between components and data flows easier to understand at a glance.

## How I Interpreted User Needs and Implemented Them Into the Design
I interpreted the user’s needs as reliability, cross-platform access, and a smooth gameplay experience during real-time rounds. I translated those needs into design choices such as a server-authoritative web service, HTTPS-based communication, real-time update support (e.g., WebSockets), centralized state storage, and strong security practices. Considering user needs is critical because the “best” technical design is only successful if it supports usability, performance, and trust for the people playing the game.

## My Approach to Designing Software and Future Strategies
I approached the design by first identifying functional requirements (game rules, team/player management, unique naming) and then evaluating platform constraints and tradeoffs (operating systems, scalability, storage, memory, security). In the future, I would continue using a structured approach that includes: requirements analysis, architectural pattern selection (n-tier, stateless services), risk assessment (failure points, outages), and validation of design decisions against scalability and security needs.
