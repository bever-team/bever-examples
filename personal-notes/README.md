# Personal notes

Private records: everyone sees, changes, and deletes only their own notes.

- `Action Create, Read, Update, Delete Note By Owner` on a `Field Owner -> Identity`.
- On `Create`, the rule means people can only create notes they own, so the app fills in Owner for them.
- On `Read`, the rule filters every list to the signed-in account's notes. Opening someone else's note by URL returns `403 Forbidden`.
- Notes are edited in a dialog (`Editing Mode Modal`).

## Try it

Register two accounts in two browsers. Each sees only their own notes.
