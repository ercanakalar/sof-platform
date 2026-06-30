Decision: Use a Cargo workspace in a monorepo.
Context: We expect multiple applications, shared libraries, firmware, and simulations to evolve together.
Alternatives considered: Multiple repositories, a single Rust package, separate workspaces.
Consequences: Simpler dependency management, shared tooling, unified CI/CD, but a larger repository to manage.