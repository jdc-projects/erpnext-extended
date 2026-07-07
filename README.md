# erpnext-extended

Extended ERPNext Docker image for project-specific additions.

## Extensions

- [`frappe-oidc-extended`](https://github.com/MohammedNoureldin/frappe-oidc-extended)

## Image

Images are published to GitHub Container Registry:

```text
ghcr.io/jdc-projects/erpnext-extended
```

Tags include both the ERPNext version and the extension version:

```text
erpnext-<erpnext-version>-oidc-<frappe-oidc-extended-version>
```

For example:

```text
ghcr.io/jdc-projects/erpnext-extended:erpnext-v15.65.2-oidc-v1.0.0
```

## Building

Run the `Create and publish an ERPNext Docker image` workflow manually and provide:

- `erpnext_version`: tag from `frappe/erpnext`
- `frappe_oidc_extended_version`: branch or tag from `MohammedNoureldin/frappe-oidc-extended`

The workflow validates both inputs before building and pushing the image.
