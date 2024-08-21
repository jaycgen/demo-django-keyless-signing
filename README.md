# demo-django-keyless-signing
Demo Chainguard toolset

## Verification using specific tag
```
cosign verify ghcr.io/jaycgen/demo-django-keyless-signing:sha-5f503244b545b1e7182705c96cbe4ff431992c0b \
  --certificate-identity https://github.com/jaycgen/demo-django-keyless-signing/.github/workflows/docker-publish.yml@refs/heads/main \
  --certificate-oidc-issuer https://token.actions.githubusercontent.com | jq
```