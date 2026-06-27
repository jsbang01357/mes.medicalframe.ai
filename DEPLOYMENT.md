# mes.medicalframe.ai deployment

## GitHub Pages

- Repository: `https://github.com/jsbang01357/mes.medicalframe.ai`
- Pages source: `main` branch, repository root
- Custom domain: `mes.medicalframe.ai`
- CNAME file: `CNAME`

## DNS

Set this record at the DNS provider for `medicalframe.ai`:

```text
Type: CNAME
Name: mes
Value: jsbang01357.github.io
```

After DNS resolves, enable HTTPS enforcement in GitHub Pages if it is not enabled automatically.

## Verification

```bash
dig CNAME mes.medicalframe.ai
curl -I https://mes.medicalframe.ai
```

The site has been verified by forcing `mes.medicalframe.ai` to a GitHub Pages IP with `curl --resolve`.
