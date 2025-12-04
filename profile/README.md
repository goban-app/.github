# Goban

> The modern home for Go – also known as Baduk (Korea) and Weiqi (China).

Goban is an online platform for Go / Baduk / Weiqi: a place to play, study, and stay engaged with the game across web and mobile.

This GitHub organization hosts selected backend services and tooling that power Goban.  
The core product is not fully open source, but components that are useful on their own will be maintained publicly here.

---

## What Goban is about

We want Goban to feel like a long-term home for people who care about the game:

- **New players** who finally want a clear way into Go / Baduk / Weiqi.
- **Club players** who want better tools to review games and train consistently.
- **Strong players** who value sharp analysis, clean interfaces, and meaningful competition.

Core ideas behind Goban:

- A **fast, modern experience** on web and, over time, native platforms.
- **AI-assisted learning** using strong engines such as KataGo.
- **Daily engagement** with analysis tools, puzzles, and structured study flows.
- A brand and story that help more people discover and stick with Go / Baduk / Weiqi.

---

## Public repositories

### [`katago-server`](https://github.com/goban-app/katago-server)

A high-performance REST API server for [KataGo](https://github.com/lightvector/KataGo) written in Rust.

It provides:

- Move suggestions and board analysis for Go / Baduk / Weiqi
- Rich evaluations: win rate, score estimates, principal variations, ownership maps
- A versioned `/api/v1` JSON API with robust error handling (RFC 7807)
- Async processing, structured logging, and health checks
- Docker images suitable for CPU deployments (and extensible for GPU)
- Kubernetes-friendly deployment via containers and configuration files

This service is one of the analysis backbones of Goban and can also be used independently in other Go-related projects.

Each public repository in this organization includes its own README with installation, configuration, and API details.

---

## How we build

Even if only parts of the stack are public, we treat the whole system with the same standards:

- **Test-first mindset** – features ship with tests; reliability is not optional.
- **Clean structure** – clear modules, consistent folder layouts, shared linting/formatting.
- **Performance as a feature** – low latency and predictable behaviour matter for serious play.
- **Kubernetes-native** – GitOps, Helm, and Kustomize for reproducible deployments.

The goal is a codebase that can support Goban for years without turning into a pile of tech debt.

---

## Follow the journey

Goban aims to:

- Offer a better way to **play Go / Baduk / Weiqi online**
- Make **AI-supported study** approachable for more players
- Support the growth of the global Go community

If you’re:

- A Go / Baduk / Weiqi player,
- A Rust / TypeScript / full-stack engineer,
- Or someone interested in tools for mind sports,

you’re welcome to watch this organization, star the repositories, or open issues to start a conversation.

---

## Links

- Website: https://goban.app  
- LinkedIn: https://www.linkedin.com/company/goban-app  

---

## Licensing

Licensing is defined per repository.

Some components are released under permissive licenses (for example MIT), while others may remain proprietary to Goban.  
Always refer to the `LICENSE` file in each repository for details.
