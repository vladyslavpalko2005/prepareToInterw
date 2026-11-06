# 12-week Middle Frontend Interview Roadmap

**Dates:** 2026-11-06 — 2027-01-31. **Target:** React + TypeScript Middle Frontend interviews, while exploring Full-stack fundamentals. **Pace:** 12–15 hours/week. Approximate split: 50% coding, 30% theory, 20% interview preparation.

| Week | Main focus | Deliverable | Exit criterion |
|---|---|---|---|
| 01 | JS: types, scope, closures, arrays, event loop, async | JS exercises + searchable directory | Independently solve JS tasks and explain execution |
| 02 | Browser JS, DOM, events, fetch, errors | TaskFlow v1 | Search/filter/sort, loading/error states |
| 03 | Semantic HTML/CSS, responsive design, accessibility, HTTP | Responsive TaskFlow | Keyboard access, mobile support, explain CORS |
| 04 | TypeScript: generics, narrowing, unions, strict mode | TaskFlow in TypeScript | Types without unjustified `any` |
| 05 | React: rendering, hooks, state, effects, forms | Operations Dashboard v1 | Explain render/effect loops and implement controls |
| 06 | React architecture, routing, server state | Dashboard v2 | TanStack Query, URL filters, pagination |
| 07 | Vitest, React Testing Library, Playwright, debugging | Tests + CI | Test key user journeys |
| 08 | Performance, accessibility and web security | Optimized dashboard | Profiling evidence, explain XSS/CSRF |
| 09 | Frontend system design, trade-offs and refactoring | Architecture report + dashboard | Defend design for large datasets |
| 10 | Next.js, Node/Express HTTP API, basic data flow | Booking Platform MVP | Explain browser → API → database; CRUD |
| 11 | Interview coding, React debugging, behavioral questions | Two mock interviews | Complete timed challenges and explain decisions |
| 12 | Full mocks, CV, GitHub polish and applications | Three mock interviews + portfolio | No critical gaps in core JS/TS/React |

## Three projects
1. **TaskFlow (weeks 1–4):** Vanilla HTML/CSS/JS task manager; later strict TS. CRUD, search, filters, sorting, local persistence, accessibility, mobile.
2. **Operations Dashboard (weeks 5–9, flagship):** React/TS, Router, TanStack Query, forms with validation, paginated sortable large dataset, URL state, loading/error/empty screens, test coverage, CI, performance profiling. Mock API/MSW is acceptable.
3. **Booking Platform (weeks 10–12):** Next.js frontend with basic Node/Express REST API. Booking CRUD, availability validation and HTTP errors; PostgreSQL optional. No payments required.

## Weekly cadence
Mon–Thu 1.5 h daily; Fri 1 h review; Sat 4 h project; Sun 3 h tests/mock/review (14 h total).

## Evidence gates
A task is DONE only after criteria and meaningful edge cases pass. A skill is VERIFIED only after an independent no-hints exercise and explanation. At weeks 4, 8, 12 use mock assessment /100: JS/TS 25, React/architecture 25, live coding 20, browser/HTTP/testing 15, system design/communication 15. Target 80+ without a critical core deficiency; this is an internal rubric, not a hiring guarantee.