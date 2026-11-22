# Contributing to EDWIN

Thank you for your interest in contributing to **EDWIN**! 

## Code of Conduct
Please ensure a respectful, collaborative, and inclusive environment. Avoid harmful or abusive behavior.

## How to Contribute
1. **Fork the repository** on GitHub.
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/<your-username>/EDWIN.git
   ```
3. **Create a feature branch**:
   ```bash
   git checkout -b feat/your-feature-name
   ```
4. **Make and verify your changes**:
   * Frontend: Run `npm run lint` and `npm run typecheck` inside `frontend/`.
   * Backend: Run `pytest` and `ruff check .` inside `backend/`.
5. **Commit with conventional commit messages**:
   ```bash
   git commit -m "feat(agents): add rate-limiting fallback to research swarm"
   ```
6. **Push to your fork and submit a Pull Request** against `main`.

## Reporting Security & Privacy Issues
Due to the biometric and OSINT nature of this software, please report vulnerabilities or ethical concerns directly via private issue or maintainer security contacts.