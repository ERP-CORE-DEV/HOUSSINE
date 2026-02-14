# EAGLES Kickoff — HOUSSINE

## Assigned Microservice: [5.11] Reporting & Analytics

**Repo**: [rh-optimerp-reporting-and-analytics](https://github.com/ERP-CORE-DEV/rh-optimerp-reporting-and-analytics)
**Issue**: [#15](https://github.com/ERP-CORE-DEV/rh-optimerp-reporting-and-analytics/issues/15)

---

## Phase 1 — Plan (uses 1 planner agent, isolated context)
```
/plan reporting-and-analytics microservice — Controller-Service-Repository, .NET 8, CosmosDB SDK 3.54, React 18 + Ant Design, French HR compliance (bilan social, index egalite, BDESE). Reference: rh-optimerp-sourcing-candidate-attraction repo.
```

## Phase 2 — Scaffold (after plan approval)
```
/scaffold reporting-and-analytics
```

## Phase 3 — TDD first feature
```
/tdd hr-dashboard-reporting
```

## Phase 4 — Pre-PR validation
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
- **French HR**: Bilan social, index egalite professionnelle, BDESE reporting
- **Tests**: xUnit + FluentAssertions + Moq, minimum 80% coverage
- **Commits**: Conventional commits (feat/fix/refactor/test/docs)
- **Integration dependencies**: Watches [5.8] Talent Management and [5.10] HR Digitalization

## Reference Repo
Use [rh-optimerp-sourcing-candidate-attraction](https://github.com/ERP-CORE-DEV/rh-optimerp-sourcing-candidate-attraction) as the architecture reference.
