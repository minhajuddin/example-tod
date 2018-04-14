title: The dot iex file
tags:
 - elixir
 - iex
 - beginner
---

If you use the `iex` repl a lot, you should alias your modules and import your utility
functions

```
# .iex.exs

alias MyApp.Repo
alias MyApp.Accounts.User

get_user = fn -> Repo.one(from u in User, limit: 1) end
```
