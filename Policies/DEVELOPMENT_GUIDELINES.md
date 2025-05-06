# Ubivera Engineering Standards & Development Policy (v1.0)

This document outlines the software development standards and technical architecture principles to be followed by all contributors and team members working on Ubivera projects.

---

## 1. Language and Platform Standards

- All **backend services** must be written in **C# (.NET)** using the latest stable LTS version (**.NET 9.0**+).
- All code must follow **Clean Architecture** principles, emphasizing separation of concerns, testability, and modularity.
- Async, DI (dependency injection), and cancellation tokens must be leveraged for all I/O-bound operations.

---

## 2. Frontend Standards

- All non-stylistic frontend programming must be written in **Typescript**.
- When a frontend framework is required, the preferred stack is **Angular (v19+)**.
    - Use standalone components with proper encapsulation and OOP-style service abstraction.
    - React or Blazor may be approved as alternatives by exception, but Angular is the assumed default.
- Styling should prioritize accessibility (WCAG 2.1), responsiveness, and semantic HTML.

---

## 3. Testing and Quality

- Every project must include:
    - Unit test coverage ≥ 80% for application logic
    - At least one integration test per external dependency
    - At least one sample project showcasing how another developer would use your design
- Prefer xUnit for .NET, Jasmine/Karma for Angular

---

## 4. DevSecOps & Git Practices

- All repositories must use:
    - Branch protection
    - Signed commits
    - GitHub Secrets for config
- Do not commit any credentials, secrets, or hardcoded endpoints
- Use GitHub Issues for tracking all tasks, bugs, and improvements