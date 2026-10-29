# Bever examples

Complete [Bever](https://bever.dev) models, each with a short explanation of what it demonstrates.

> **Bever is pre-alpha.** The language and APIs will change in breaking ways between releases, and there is no upgrade path yet. Do not use it for production data. See [Status](https://bever.dev/guide/what-is-bever#status).

| Example | Shows |
| --- | --- |
| [task-board](task-board) | The starter model: projects, tasks, sign-up, and assignees |
| [order-desk](order-desk) | The [tutorial](https://bever.dev/guide/tutorial) app: customers, products, orders, and owner-only edits |
| [personal-notes](personal-notes) | Private records: everyone sees only their own notes |
| [product-catalog](product-catalog) | A public catalog that anyone can browse and signed-in staff edit inline |
| [help-desk](help-desk) | Pickers that differ from reading, a named picker, a modal picker, and a role |

## Run an example

You need the [Bever CLI](https://bever.dev/guide/getting-started) (`dotnet tool install --global --prerelease Bever.Cli`).

```sh
git clone https://github.com/bever-team/bever-examples
bever new "Help Desk"
cp bever-examples/help-desk/bev/*.bev "Help Desk/bev/"
rm "Help Desk/bev/app.bev"
cd "Help Desk"
bever dev
```

Copy the model before the first `bever dev`, so the first database is created from it.

## Contributing

New examples are welcome when they show something the others do not. Each example is a folder with `bev/*.bev` and a `README.md` that says what it demonstrates and how to try it. `bever check <folder>/bev` must pass; CI checks every example.

## License

Licensed under [MIT No Attribution](LICENSE). Copy the models into your own projects without keeping a notice. "Bever" and the Bever logo are trademarks; see [TRADEMARKS.md](https://github.com/bever-team/bever/blob/main/TRADEMARKS.md).
