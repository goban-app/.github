# Goban

> The modern home for Go – also known as Baduk (Korea) and Weiqi (China).

Goban is a modern online platform for Go / Baduk / Weiqi: a place to play, study, and stay engaged with the game.

This GitHub organization hosts selected services and tools that power Goban.  
The core product is not fully open source, but when a component is useful on its own, we aim to maintain it publicly here.

---

## What Goban is about

We want Goban to feel like a home for everyone who cares about the game:

- **New players** who have seen the board, but never had a clear way to learn.
- **Club players** who want better tools to review games and train regularly.
- **Strong players** who value sharp analysis, clean interfaces, and good competition.

Our focus:

- A clean, fast experience on **web, mobile, and eventually desktop**.
- **AI-assisted learning** powered by strong engines like KataGo.
- **Daily engagement** through puzzles, analysis tools, and structured study.
- A brand and story that help more people discover and stick with Go / Baduk / Weiqi.

---

## Code in this organization

This org will gradually contain selected components of the Goban stack, for example:

### KataGo-based analysis service

A production-ready HTTP API around [KataGo](https://github.com/lightvector/KataGo), used within Goban for:

- Post-game review with suggested moves
- Position analysis and win-rate graphs
- Generating and validating puzzles / tsumego

Key characteristics:

- Implemented in Rust with an async, high-performance web stack
- Versioned JSON APIs with structured error handling
- First-class observability: logging, metrics, health checks
- Containerized for CPU / GPU and deployable via Helm to Kubernetes

Other public repositories will document their own architecture, APIs, and usage in their respective `README.md` files.

---

## How we build

Even if only parts of the code are public, we care a lot about how the whole system is built:

- **Test-driven mindset** – features ship with tests; reliability is a requirement.
- **Clean structure** – clear modules, consistent folder layouts, and shared linting/formatting.
- **Performance as a feature** – low latency and predictable behaviour matter as much as visuals.
- **Kubernetes-native deployments** – GitOps, Helm, and Kustomize for reproducible rollouts.

This keeps the codebase maintainable over the long term and makes it easier to evolve Goban without accumulating unnecessary debt.

---

## Follow the journey

Goban aims to:

- Offer a better way to **play Go / Baduk / Weiqi online**.
- Make **AI-supported study** accessible and approachable.
- Contribute to the growth of the global Go community, not just serve existing players.

If you’re:

- A Go / Baduk / Weiqi player,
- A Rust / TypeScript / full-stack engineer,
- Or someone who cares about tools for mind sports,

you’re welcome to watch this organization, star the repos, or open issues to start a conversation.

---

## Licensing

Licensing is defined per repository.

Some components will be released under permissive licenses (for example MIT or Apache-2.0), while others may remain proprietary to Goban.  
Always refer to the `LICENSE` file in each repository for details.
