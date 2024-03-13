# rebase-push-action
Basically this is doing git rebase &amp;&amp; git push

```yaml
on:
  workflow_dispatch:

jobs:
  rebase-push:
    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v4
    - uses: touchground/rebase-push-action@main
      with:
        repo: '<username>/<repo>'
        branch: 'main'
        message: 'Rebase and push to main'
```
