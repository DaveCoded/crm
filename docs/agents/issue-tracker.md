# Issue tracker: Linear

Project: [Personal CRM](https://linear.app/dave-bernhard/project/personal-crm-361b99d93eee) (`P-DAV-1`). Team: `DAV`.

Use the connected Linear tools to read and write issues in this project. When the connection is unavailable, use the same project in the Linear UI.

## Conventions

- Create specs as project issues titled `Spec: <name>`. Their full bodies contain the spec; implementation tickets can be child issues.
- Create implementation tickets as project issues. Use a parent issue when they come from a spec or decision map. Use Linear's native blocking relations for dependencies.
- Use triage labels to show readiness; use Linear statuses for progress. The team currently has Backlog, Todo, In Progress, Done, Canceled, and Duplicate.
- Read issue descriptions, comments, labels, parent links, and blocking relations before continuing existing work.
- When a skill says “publish to the issue tracker,” create an issue in this project. When it says “fetch the relevant ticket,” open the Linear issue by ID or URL.

## Wayfinding operations

- Map: a project issue labeled `wayfinder:map` with Destination, Notes, Decisions so far, Not yet specified, and Out of scope sections.
- Decision tickets: child issues of the map, labeled `wayfinder:research`, `wayfinder:prototype`, `wayfinder:grilling`, or `wayfinder:task`.
- Blocking: use native Linear `blockedBy` relations. The frontier is open, unassigned child issues with no open blockers.
- Claim: assign the chosen ticket to yourself before work.
- Resolve: add the answer as a comment, move the ticket to Done, and append a one-line link to the map's Decisions so far.
