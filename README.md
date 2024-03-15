# push-action
Pushes to a remote repository, and if there is a failure, tries pull with fast-forward first before pull with merge and then rebase

```yaml
on:
  workflow_dispatch:

jobs:
  rebase-push:
    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v4
    - uses: touchground/push-action@main
```
