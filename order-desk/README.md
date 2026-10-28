# Order desk

The app built in the [tutorial](https://bever.dev/guide/tutorial): customers, products, and orders.

- `Email` and `Phone` fields with format checks, `Money` and `Int` fields, and enum defaults.
- `Field Customer -> Customer` with the default `OnDelete Restrict`: a customer with orders cannot be deleted.
- `Action Update, Delete Order By SalesRep`: everyone sees every order, only its sales rep changes it.
- `Present` with a record label, a renamed field, chosen list columns, modal editing, and a dropdown picker.

## Try it

Register two accounts. Create an order with the first account as sales rep, then sign in as the second: the order is listed, but Edit and Delete are not offered, and the API refuses them.
