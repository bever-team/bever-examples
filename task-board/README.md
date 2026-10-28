# Task board

The model that `bever new` starts with: projects and tasks, with self-service sign-up.

- `Identity` with `Registration Enabled` lets people create accounts in the app.
- `Field Project -> Project OnDelete Cascade` deletes a project's tasks with it.
- `Field Assignee -> Identity?` references an account; the app picks accounts by email.
- Enums with defaults (`Status`, `Priority`) and an optional `Date`.
- `Present Listing` chooses the task list's columns; `OrderBy DueDate` sorts it.

## Try it

Create an account, add two projects, then add tasks to them. Delete a project and its tasks disappear too.
