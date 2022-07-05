# Checkout Action

This repository wraps the [actions/checkout](https://github.com/actions/checkout) and adds the following features:
- Provide a clean environment for non-ephemeral self-hosted Github Action runners
- Checkout a private repository containing custom actions

# Usage

```yaml
- uses: john-jam/checkout-action@v1
  with:
    # The private actions repository to checkout in the .github/actions folder
    actions-repo: ""

    # The ssh deploy key used to clone the actions private repository
    actions-ssh-key: ""
```