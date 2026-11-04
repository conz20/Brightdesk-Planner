# Brightdesk Planner

<p align="center"><img src="assets/branding/mark.svg" width="82" height="82" alt="Brightdesk brand mark"><br><strong>brightdesk</strong></p>
<p align="center"><img src="assets/branding/icons/planner.svg" width="112" height="112" alt="Brightdesk Planner application icon"></p>

<p align="center"><strong>Plan projects, organise tasks and track progress.</strong></p>

<p align="center"><img src="assets/previews/planner.svg" width="100%" alt="Brightdesk Planner workspace design preview"></p>

> **Visual example:** This is the proposed Brightdesk Planner experience. It is a design concept, not a screenshot of a finished application.

## Shared Brightdesk design standard

The planned product follows the [Brightdesk visual and interaction standard](https://github.com/connormolloy12/Brightdesk-suite/blob/main/docs/BRIGHTDESK_VISUAL_STANDARD.md) for branding, icon usage, layout, responsive behaviour and accessibility.

## Product experience

Brightdesk Planner is planned as a local-first project planning workspace with boards, timelines, tasks, priorities and progress tracking.

## Planned capabilities

- Create plans, buckets and task cards.
- Track due dates, priorities and progress.
- Switch between board and timeline views.
- Search and filter plans.
- Keep project data on this device.

## Implementation status

**Repository scaffold only.** This repository contains product design assets and documentation, but no runnable application source, package manifest, automated app tests or desktop installer. Do not treat the concept preview as a working app.

## Design brief

See [docs/DESIGN_BRIEF.md](docs/DESIGN_BRIEF.md) for the planned screens, navigation and acceptance targets.

## Related project

[Brightdesk Office Suite](https://github.com/connormolloy12/Brightdesk-suite)

## Professional workspace examples and acceptance

Planner should provide a clear overview of work, ownership, timing and progress. The main example should show a realistic project board with task cards, owners, due dates and progress—not a decorative collection of empty columns.

### Example workflow

1. Create a project plan with a few work stages.
2. Add tasks with owners, priorities and due dates.
3. Move a task between stages and update its progress.
4. Switch between board and timeline views where implemented.
5. Filter the plan to focus on overdue or high-priority work.

Make status and priority understandable without relying on colour alone. Keep task cards consistent, dates readable and the relationship between board and timeline views clear. Do not present unimplemented collaboration, notifications or cloud sync as available.

Follow the shared [Brightdesk visual and interaction standard](https://github.com/connormolloy12/Brightdesk-suite/blob/main/docs/BRIGHTDESK_VISUAL_STANDARD.md).

### Acceptance checks

- Task creation, status changes, ownership and due dates are represented accurately.
- Board and timeline views remain consistent when switching, if both are shipped.
- Keyboard access, focus, contrast and non-colour status cues are checked.
- Scaffold status is not confused with a runnable application.
