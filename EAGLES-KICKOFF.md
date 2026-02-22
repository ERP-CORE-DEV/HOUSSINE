# EAGLES Kickoff - HOUSSINE

## Assigned Microservice: [5.3] Hiring Management

**Repo**: [rh-optimerp-hiring-management](https://github.com/ERP-CORE-DEV/rh-optimerp-hiring-management)
**Syncs with**: LAHCEN (5.2 Candidate Evaluation) upstream

---

## Phase 1 - Plan (uses 1 planner agent, isolated context)
```
/plan hiring-management microservice - Controller-Service-Repository, .NET 8, CosmosDB SDK 3.54, React 18 + Ant Design, French HR compliance (promesse d embauche, DPAE, contrat de travail, periode d essai, convention collective). Reference: rh-optimerp-sourcing-candidate-attraction repo.
```

## Phase 2 - Scaffold (after plan approval)
```
/scaffold hiring-management
```

## Phase 3 - TDD first feature
```
/tdd interview-scheduling-workflow
```

## Phase 4 - Pre-PR validation
```
/code-review
/security-scan
/gdpr-check
```

---

## Key Rules
- **Pattern**: Controller-Service-Repository (NOT CQRS/MediatR)
- **Database**: CosmosDB SDK 3.54 direct (NOT EF Core)
- **GDPR**: AnonymizeXxx() on personal data models + IsAnonymized flag
- **French HR**: Promesse d embauche, DPAE, contrat de travail, periode d essai, convention collective
- **Tests**: xUnit + FluentAssertions + Moq, minimum 80% coverage
- **Commits**: Conventional commits (feat/fix/refactor/test/docs)
- **Integration dependencies**: Watches [5.2] Candidate Evaluation and [5.4] Legal and Regulatory Compliance

## Reference Repo
Use [rh-optimerp-sourcing-candidate-attraction](https://github.com/ERP-CORE-DEV/rh-optimerp-sourcing-candidate-attraction) as the architecture reference.
