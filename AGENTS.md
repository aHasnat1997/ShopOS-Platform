# ShopOS-Platform

This file provides context about the project for AI assistants.

## Project Overview

- **Ecosystem**: Typescript

## Tech Stack

- **Runtime**: bun
- **Package Manager**: bun

### Frontend

- Framework: astro, native-bare
- CSS: tailwind

### Backend

- Framework: nestjs
- API: ts-rest
- Validation: zod

### Database

- Database: postgres
- ORM: prisma

### Additional Features

- Job Queue: bullmq
- Logging: winston

## Project Structure

```
ShopOS-Platform/
├── apps/
│   ├── web/         # Frontend application
│   ├── native/      # Mobile application (React Native)
│   └── server/      # Backend API
├── packages/
│   ├── api/         # API layer
│   └── db/          # Database schema
```

## Common Commands

- `bun install` - Install dependencies
- `bun dev` - Start development server
- `bun build` - Build for production
- `bun db:push` - Push database schema
- `bun db:studio` - Open database UI

## Better Fullstack project context

`bts.jsonc` is the authority for the current Stack Graph. Its `stackParts` array owns role selection and `ownerPartId` bindings. Top-level option fields are a compatibility projection and must not become a second mutation path.

### Stack Parts, ownership, and evidence

- `backend.api:typescript:ts-rest`. It belongs to `backend:typescript:nestjs`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `backend.jobQueue:typescript:bullmq`. It belongs to `backend:typescript:nestjs`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `backend.logging:typescript:winston`. It belongs to `backend:typescript:nestjs`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `backend.orm:typescript:prisma`. It belongs to `backend:typescript:nestjs`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `backend.runtime:typescript:bun`. It belongs to `backend:typescript:nestjs`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `backend.validation:typescript:zod`. It belongs to `backend:typescript:nestjs`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `backend:typescript:nestjs`. Its generated target is `apps/server`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `database:universal:postgres`. Its generated target is `packages/db`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `developerEnvironment:universal:devcontainer`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `frontend.css:typescript:tailwind`. It belongs to `frontend:typescript:astro`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `frontend.forms:typescript:react-hook-form`. It belongs to `frontend:typescript:astro`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `frontend:typescript:astro`. Its generated target is `apps/web`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `mobile.navigation:react-native:expo-router`. It belongs to `mobile:react-native:native-bare`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `mobile:react-native:native-bare`. Its generated target is `apps/native`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.
- `workspaceRunner:universal:turborepo`. Evidence is `listed` with `unverified` freshness. Verification maintainer: @Marve10s.

### Installed-version authority

Use `bts.jsonc` for the generator and schema version. Use local package manifests and lockfiles for installed dependency versions. Do not assume that documentation for a newer Better Fullstack release matches this project.

### Compatibility and lifecycle safety

Run `create-better-fullstack context --json` for bounded roles, capabilities, evidence, compatibility issues, and safe next actions. Run `create-better-fullstack doctor --json` before repairing graph drift. Existing-project writes must start with a plan and use the exact review token. Use `create-better-fullstack recipes check --json` before editing recipe-owned paths or managed regions, and use recipe history plus project recovery commands to undo a reviewed operation.

User code outside an explicit Better Fullstack managed region is not generator-owned. Missing or changed managed-region hashes stop recipe planning for manual review.

<!-- <better-fullstack:recipes sha256=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855> -->

<!-- </better-fullstack:recipes> -->

## Maintenance

Keep AGENTS.md updated when:

- Adding/removing dependencies
- Changing project structure
- Adding new features or services
- Modifying build/dev workflows

AI assistants should suggest updates to this file when they notice relevant changes.
