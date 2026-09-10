# Directive — Working Context and Handoff

**Updated:** 7 September 2026

Use this file to resume the project in a new chat or work session without repeating discovery.

## Current state

- Product specification is complete: [project-plan.md](project-plan.md).
- Production roadmap is complete: [implementation-plan.md](implementation-plan.md).
- Jira starter backlog is available: [jira-backlog.csv](jira-backlog.csv).
- `project-plan.md` contains the consolidated decisions.
- No application code has been created.
- The workspace is a Git repository.
- Jira, cloud, Apple, Google Play, Expo, email, analytics, or monitoring account has been connected in this session.

## Confirmed product decisions

- Adults 18+: working adults, adult students, and people who frequently forget commitments.
- Android, iOS, and web; English first; global ambition with country/capability gating.
- Own app/chat and push are primary; Telegram optional; other messaging channels deferred or conditional.
- Bounded scheduling autopilot, explainable changes, undo, user-controlled Boss Mode, quiet hours, and emergency escape.
- Free basics and paid AI/advanced automation.
- Assumed team size: 2–4 builders.
- Calls and financial stakes are later, separately gated features.

## Recommended technical direction

- TypeScript monorepo: Next.js web, Expo/React Native mobile, Fastify API and worker.
- Managed PostgreSQL, durable managed job queue, object storage, managed authentication, Terraform, GitHub Actions.
- Built arround platform focus controls.
- Modular monolith until measured scale or ownership requires separation.
- Target 10,000 MAU; load-test notification bursts and AI cost rather than overbuilding infrastructure.

## Verified local environment

- Node.js 24.18.0; npm 12.0.2; Git 2.54.0.
- Docker Desktop 29.4.0 is running; WSL Ubuntu is present.
- Android Studio and Android SDK are installed.
- Android Studio ships JDK 21; PATH currently selects Java 8.
- Mac and iPhone availability: _present_

## Answers still needed

Fill these in before repository/cloud/account setup:

- **Monthly beta infrastructure/services budget (excluding salaries and one-time legal/security work):** _Starting with Free_
- **Named team members and roles:** _Akshat7, JagerMeister, Akshat, Boho_
- **Mac and physical iPhone available:** _Available_
- **GitHub organization/repository URL:** _https://github.com/AkshatTandekar07/Directive_
- **Jira site/project URL and preferred project key:** _https://tandekarakshat7.atlassian.net?continue=https%3A%2F%2Ftandekarakshat7.atlassian.net%2Fwelcome%2Fsoftware&atlOrigin=eyJpIjoiODEwZWU0MWQ1ZTk1NGE4ZDgwOTNhZTViZDRmZGViMjAiLCJwIjoiaiJ9; suggested key `DIR` TBD_
- **Preferred cloud provider and billing account:** _TBD; implementation plan currently assumes serverless deployment model_
- **Primary launch/data region:** _India_
- **Organization-owned domain/email:** _TBD_

## Exact next session prompt

> Continue Directive from `project-context.md`. Read `project-plan.md` and `implementation-plan.md`. Use my completed answers in the context file. Check up the Git repository, monorepo, local development environment, CI, ADRs, and first vertical-slice backlog. Do not create paid external resources without showing the concrete configuration and cost first.

## Guardrails

- Do not call planned app features implemented.
- Do not put secrets in the repository or chat.
- Do not enable external sends, partner alerts, or device enforcement without the specified consent.
- Do not expand the first release to deferred integrations before the vertical slice and native risk prototypes pass.
- Recheck current provider policies/pricing before implementation.
