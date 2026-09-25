# Copilot Instructions

## Code Review Focus

When reviewing pull requests, focus **exclusively** on:

1. **Security vulnerabilities** — injection (SQL, command, LDAP, XPath), XSS, CSRF, insecure deserialization, broken authentication, secrets/credentials in code, path traversal, unsafe redirects, insecure dependencies.
2. **Correctness bugs** — logic errors, null/undefined dereferences, off-by-one errors, race conditions, incorrect error handling, data loss paths.

## Context from Linked Issues and Work Items

When the PR body references an issue (e.g., `Closes #123`, `Fixes #456`) or an Azure DevOps work item (e.g., `AB#123`), read its full context before reviewing:

- The issue or work item **description** — to understand the intended behavior and acceptance criteria.
- All **comments** on the issue — to capture clarifications, decisions, and scope changes made during discussion.
- Any **attached files** (specs, screenshots, diagrams) — to validate that the implementation matches the agreed design.

Use this context to judge whether the diff correctly and safely implements what was specified. If the linked context reveals that the change is incomplete or contradicts an agreed constraint, flag it as a correctness finding.

## Scope Constraint

- Review **only** lines that were added or modified in the diff.
- Do not comment on unchanged code unless it creates a direct security or correctness risk when combined with the new changes.
- Do not suggest style improvements, refactors, naming changes, or performance optimizations.
- Do not flag speculative issues — only report findings with a clear, concrete failure scenario.

## Output Format

Todos os comentários devem ser escritos em **português brasileiro**.

Para cada problema encontrado:
- Aponte a **linha específica**.
- Explique em uma frase curta **por que é um problema** — qual risco concreto isso representa (o que quebra, vaza ou permite exploração).
- Sugira o **fix mínimo** necessário para resolver — nada além disso.

Se não houver problemas de segurança ou correção no diff, diga isso de forma breve e direta. Não preencha a revisão com observações neutras.
