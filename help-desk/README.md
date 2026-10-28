# Help desk

Pickers that differ from reading, and a role.

- Customers are private to the agent who owns them (`Read ... By Owner`), but `Action Pick Customer By Authenticated` lets every agent choose any customer for a ticket. Pickers return only names, never full records.
- `Action Pick Team As Mine By Lead` is a named picker, and `Field Team -> Team Pick Mine` uses it: tickets can only be filed under teams you lead.
- `SearchBy Name, Email` makes the customer picker search both fields; `Input Customer Picker Modal` opens it in a dialog.
- `OrderBy Priority Desc` lists urgent tickets first, in the enum's declared order.
- `Role Supervisor` declares a role. `Read Customer By Supervisor` lets supervisors see every customer, and `Delete Ticket By Supervisor` makes deleting tickets theirs alone.

## Try it

Register two agents. The first creates a customer and a team they lead. The second cannot open the customer, but can choose it on a new ticket; their team picker is empty because they lead no team.

Make the first agent an Administrator with `bever identity admin add --email <email>`. Signed in, they get a *People* page where they can make the second agent a Supervisor; the second agent then sees every customer and can delete tickets. `bever identity role add --email <email> --role Supervisor` does the same from the command line.
