# git git-symbolic-ref

> Read, change or delete named references.
> More details - and why it's named symbolic: <https://git-scm.com/docs/git-symbolic-ref>.

- Add or update a reference

`git symbolic-ref {{name}} {{ref}}

- Add or update, including a message to explain the reason

`git symbolic-ref -m "{{message text}}" {{name}} {{ref}}

- Delete a reference. Reason can not be added.

`git symbolic-ref --delete {{name}}

- Additional command options:
  - --quiet - For use in scripting, to get non-zero exit code instead of showing an error if {{ref}} does not exist.
  - --short - To shorten printed names from e.g. refs/heads/branchName to branchName
