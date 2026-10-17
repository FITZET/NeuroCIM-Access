# NeuroCIM Access Portal

GitHub Pages registration portal for the private NeuroCIM Windows distribution.

## Administrator setup

1. Create the private `Lowpower-Lab/NeuroCIM-Distribution` organization repository.
2. Create a fine-grained PAT limited to that repository with **Administration: write**.
3. Add it to this repository as the Actions secret `DISTRIBUTION_ADMIN_TOKEN`.
4. Create labels: `access-request`, `pending`, `approved`, and `revoked`.
5. Enable GitHub Pages with **GitHub Actions** as the source.

Adding `approved` to an access request invites the Issue author to the distribution repository with read-only permission. Adding `revoked` removes that permission.
