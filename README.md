# just-action

This is a simple GitHub Action that runs ``just --fmt --check`` for all .just files in the repository, making sure that broken justfiles never make it to production.

## Sample usage

```yml
- name: Checkout repository code
  uses: actions/checkout@v4
- name: Check just syntax
  uses: ublue-os/just-action@v2
```

Note: the checkout action before ``just-action`` is required. 
