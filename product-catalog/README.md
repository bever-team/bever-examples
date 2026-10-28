# Product catalog

A public catalog: anyone can browse it without an account, and signed-in staff maintain it.

- `Action Read Product By Anyone` makes the catalog public. Visitors see products and categories but no New, Edit, or Delete controls.
- `Identity` without `Registration Enabled`: staff accounts are created from the command line.
- New products open in a dialog (`Creating Mode Modal`); prices are edited inside the list row (`Editing Mode Inline`).
- `Field Category -> Category? OnDelete SetNull` keeps products when their category is deleted.

## Try it

After the first `bever dev`, create a staff account in another terminal, then sign in at `/sign-in`:

```sh
bever identity bootstrap --email staff@example.com
```
