# OpenG7 Health Supply Corridors

![OpenG7 Health Supply Corridors](assets/openg7-health-supply-corridors.png)

Open-source platform for mapping critical medical supplies, distribution dependencies, and health system supply corridors.

## Investor Pitch

OpenG7 Health Supply Corridors turns fragile supply visibility into a usable operational system. Instead of depending on siloed inventories, delayed updates, and fragmented procurement coordination, teams get a shared product layer for understanding medical inputs, shortage risks, and distribution corridors.

Funding this repository helps deliver:
- Decision-grade visibility across critical supplies, distribution paths, and shortage risks
- A vendor-neutral stack built on Angular, shared API contracts, and open operational models
- Faster coordination through alerting, corridor mapping, and critical-input dashboards
- A stronger bridge between procurement teams, logistics operators, and health system planners

Near-term funding unlocks:
- Better mapping of critical inputs and route dependencies
- Stronger shortage risk indicators and operational alerts
- More resilient import, search, and monitoring workflows
- Hardening of tooling for real-world supply coordination and resilience

How to support:
- GitHub Sponsors
- Pilot partnerships
- Public-sector collaboration
- Supplier and logistics partnerships
- In-kind infrastructure or expert review

---

**Languages:** [English](#english) | [Français](#francais)

<a id="english"></a>

## English

### What it is

OpenG7 Health Supply Corridors is an open-source repository for a medical supply visibility and corridor coordination platform. It is designed to make supply dependencies and critical input risks easier to understand across regions, facilities, suppliers, and routes.

The repository is intended to support:
- an Angular front-end for supply maps, critical input dashboards, and alert surfaces
- shared contracts for products, risks, facilities, routes, and supply events
- operator-facing workflows for supply monitoring, shortage analysis, and escalation
- documentation for governance, resilience modeling, and data boundaries

This project is not an ERP replacement and not a procurement system of record. It is a coordination and observability layer.

### Why it exists

Health supply resilience often breaks where information is fragmented: local stock visibility is incomplete, dependency chains are unclear, procurement signals are delayed, and alternative routing options are hard to compare.

OpenG7 Health Supply Corridors exists to provide:
- a unified product surface for visualizing critical supply flows
- structured visibility on shortage risks and corridor fragility
- reusable contracts, selectors, and operational models
- a documented foundation that can evolve across institutions and jurisdictions

### What it enables

- Critical medical input mapping
- Distribution corridor visualization
- Shortage risk indicators
- Supplier and dependency awareness
- Route disruption monitoring
- Alternative corridor analysis

### Repository Structure

- `src/app/core/`: app bootstrap, providers, config, routing, guards
- `src/app/shared/`: UI primitives, helpers, reusable models
- `src/app/features/health-supply-corridors/`: health supply corridor domain
- `src/app/features/health-supply-corridors/pages/`: page-level shells
- `src/app/features/health-supply-corridors/components/`: maps, dashboards, alerts, risk panels
- `src/app/features/health-supply-corridors/data-access/`: API clients, adapters, supply DTOs
- `src/app/features/health-supply-corridors/store/`: global state integration when needed
- `src/app/features/health-supply-corridors/signals/`: local signal-first orchestration
- `docs/`: onboarding, architecture, supply models, roadmap
- `packages/contracts/`: shared contracts and validation schemas
- `infra/`: deployment and infrastructure manifests

### Suggested Front-End Surfaces

- `src/app/features/health-supply-corridors/pages/health-supply-corridors-page.component.ts`
- `src/app/features/health-supply-corridors/components/supply-corridor-map/supply-corridor-map.component.ts`
- `src/app/features/health-supply-corridors/components/critical-input-dashboard/critical-input-dashboard.component.ts`
- `src/app/features/health-supply-corridors/components/shortage-risk-panel/shortage-risk-panel.component.ts`
- `src/app/features/health-supply-corridors/components/route-disruption-alerts/route-disruption-alerts.component.ts`
- `src/app/features/health-supply-corridors/components/alternative-route-analysis/alternative-route-analysis.component.ts`

### Getting Started

1. Enable Corepack and verify Yarn:
   ```bash
   corepack enable
   yarn --version
   ```
2. Install dependencies:
   ```bash
   yarn install
   ```
3. Create a local environment file if needed:
   ```bash
   cp .env.example .env.local
   ```
4. Start the web application:
   ```bash
   yarn dev
   ```
5. Run tests:
   ```bash
   yarn test
   ```

Useful repo-level scripts:
- `yarn dev`
- `yarn test`
- `yarn test:e2e`
- `yarn lint`
- `yarn typecheck`
- `yarn build`

Detailed guides live in `docs/`:
- `docs/getting-started.md`
- `docs/architecture.md`
- `docs/supply-model.md`
- `docs/operations.md`
- `docs/roadmap.md`

### Supply Resilience Surfaces

The platform is expected to support operator surfaces for supply continuity and corridor resilience.

Examples:
- critical input dashboards
- supplier dependency maps
- shortage risk boards
- route disruption alerts
- alternative route and substitution analysis

### Where does code live?

- Use `src/app/features/health-supply-corridors/` for domain UI and orchestration
- Keep local state signal-first in components and feature signals
- Use `src/app/features/health-supply-corridors/store/` only for truly global context
- Put shared contracts in `packages/contracts/`
- Keep resilience rules and non-goals documented in `docs/`

### Contributing

Read `CONTRIBUTING.md` for workflow, checks, and security expectations.
The code of conduct in `CODE_OF_CONDUCT.md` applies to all community spaces.
Support and governance details live in `SUPPORT.md`.

Community first steps:
- Use issue and PR templates
- Add screenshots for visible UI changes
- Document any supply, privacy, or operational impact
- Prefer small, testable increments with explicit domain assumptions

### License & Security

- License: MIT (`LICENSE`)
- Responsible disclosure: see `SECURITY.md`

---

<a id="francais"></a>

## Français

### Ce que c'est

OpenG7 Health Supply Corridors est un dépôt open source pour une plateforme de visibilité des intrants médicaux et de coordination des corridors d’approvisionnement. Il vise à rendre plus compréhensibles les dépendances d’approvisionnement et les risques sur les intrants critiques entre régions, établissements, fournisseurs et routes.

Le dépôt a pour but de soutenir :
- un front Angular pour les cartes d’approvisionnement, tableaux de bord d’intrants critiques et surfaces d’alerte
- des contrats partagés pour les produits, risques, établissements, routes et événements d’approvisionnement
- des parcours opérateurs pour le suivi des approvisionnements, l’analyse de pénurie et l’escalade
- une documentation sur la gouvernance, la modélisation de résilience et les frontières de données

Ce projet n’est ni un remplacement d’ERP ni un système de procurement de référence. C’est une couche de coordination et d’observabilité.

### Pourquoi ce projet existe

La résilience d’approvisionnement en santé se brise souvent là où l’information est fragmentée : visibilité locale incomplète des stocks, chaînes de dépendance floues, signaux d’achat retardés et difficulté à comparer les routes alternatives.

OpenG7 Health Supply Corridors sert à fournir :
- une surface produit unifiée pour visualiser les flux d’intrants critiques
- une visibilité structurée sur les risques de pénurie et la fragilité des corridors
- des contrats, sélecteurs et modèles opérationnels réutilisables
- une base documentée qui peut évoluer à travers les établissements et juridictions

### Ce que ça permet

- Cartographie des intrants médicaux critiques
- Visualisation des corridors de distribution
- Indicateurs de risque de pénurie
- Visibilité sur les fournisseurs et dépendances
- Suivi des perturbations de routes
- Analyse de corridors alternatifs

### Structure du dépôt

- `src/app/core/` : bootstrap applicatif, providers, configuration, routing, guards
- `src/app/shared/` : primitives UI, helpers, modèles réutilisables
- `src/app/features/health-supply-corridors/` : domaine des corridors d’approvisionnement en santé
- `src/app/features/health-supply-corridors/pages/` : shells de pages
- `src/app/features/health-supply-corridors/components/` : cartes, tableaux de bord, alertes, panneaux de risque
- `src/app/features/health-supply-corridors/data-access/` : clients API, adaptateurs, DTOs d’approvisionnement
- `src/app/features/health-supply-corridors/store/` : intégration d’état global au besoin
- `src/app/features/health-supply-corridors/signals/` : orchestration locale signal-first
- `docs/` : onboarding, architecture, modèles d’approvisionnement, roadmap
- `packages/contracts/` : contrats partagés et schémas de validation
- `infra/` : manifests de déploiement et infrastructure

### Surfaces front-end suggérées

- `src/app/features/health-supply-corridors/pages/health-supply-corridors-page.component.ts`
- `src/app/features/health-supply-corridors/components/supply-corridor-map/supply-corridor-map.component.ts`
- `src/app/features/health-supply-corridors/components/critical-input-dashboard/critical-input-dashboard.component.ts`
- `src/app/features/health-supply-corridors/components/shortage-risk-panel/shortage-risk-panel.component.ts`
- `src/app/features/health-supply-corridors/components/route-disruption-alerts/route-disruption-alerts.component.ts`
- `src/app/features/health-supply-corridors/components/alternative-route-analysis/alternative-route-analysis.component.ts`

### Pour commencer

1. Activez Corepack et vérifiez Yarn :
   ```bash
   corepack enable
   yarn --version
   ```
2. Installez les dépendances :
   ```bash
   yarn install
   ```
3. Créez un fichier d’environnement local au besoin :
   ```bash
   cp .env.example .env.local
   ```
4. Lancez l’application web :
   ```bash
   yarn dev
   ```
5. Lancez les tests :
   ```bash
   yarn test
   ```

Scripts utiles à la racine :
- `yarn dev`
- `yarn test`
- `yarn test:e2e`
- `yarn lint`
- `yarn typecheck`
- `yarn build`

Guides détaillés dans `docs/` :
- `docs/getting-started.md`
- `docs/architecture.md`
- `docs/supply-model.md`
- `docs/operations.md`
- `docs/roadmap.md`

### Surfaces de résilience d’approvisionnement

La plateforme vise à supporter des surfaces opérateurs pour la continuité d’approvisionnement et la résilience des corridors.

Exemples :
- tableaux de bord d’intrants critiques
- cartes de dépendance fournisseurs
- tableaux de risque de pénurie
- alertes de perturbation de routes
- analyse de routes alternatives et substitutions

### Où vit le code ?

- Utilisez `src/app/features/health-supply-corridors/` pour l’UI métier et l’orchestration
- Gardez l’état local en signal-first dans les composants et signaux métier
- Utilisez `src/app/features/health-supply-corridors/store/` seulement pour le contexte réellement global
- Placez les contrats partagés dans `packages/contracts/`
- Conservez les règles de résilience et non-objectifs dans `docs/`

### Contribuer

Lisez `CONTRIBUTING.md` pour le workflow, les vérifications et les attentes de sécurité.
Le code de conduite dans `CODE_OF_CONDUCT.md` s’applique à tous les espaces communautaires.
Les détails de support et de gouvernance sont dans `SUPPORT.md`.

Premiers pas communautaires :
- utilisez les templates d’issues et de PR
- ajoutez des captures pour les changements UI visibles
- documentez tout impact d’approvisionnement, de confidentialité ou opérationnel
- privilégiez de petits incréments testables avec hypothèses métier explicites

### Licence & sécurité

- Licence : MIT (`LICENSE`)
- Divulgation responsable : voir `SECURITY.md`
