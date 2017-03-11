### Useful git one liners
### Show git history in one line - 
`$ git log --pretty=oneline`

`ca82a6dff817ec66f44342007202690a93763949 changed the version number`

`085bb3bcb608e1e8451d4b2432f8ecbe6306e7e7 removed unnecessary test`

`a11bef06a3f659402fe7563abf99ad00de2209e6 first commit`

### Limiting log ouput OR look for logs with specific timestamp
`$ git log --since=2.weeks`

This command works with lots of formats – you can specify a specific date
like "2008-01-15", or a relative date such as "2 years 1 day 3 minutes
ago".

e.g.
If you want to see which commits modifying test files in the Git
source code history are merged and were committed by Junio Hamano in the
month of October 2008, you can run something like this:

`$ git log --pretty="%h - %s" --author=gitster --since="2008-10-01" \`

### Show your branching history
`$ git log --oneline --decorate --graph --all`
