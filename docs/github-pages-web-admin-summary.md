# GitHub Pages DNS setup for QMM Lab website

**Site URL:** `https://qmm.labs.stonybrook.edu`  
**Purpose:** Point the Stony Brook subdomain to the QMM Lab website hosted on GitHub Pages.

## Requested DNS change

Because `qmm.labs.stonybrook.edu` is a subdomain, GitHub Pages recommends a **CNAME** DNS record, not A records.

Please create/update this DNS record:

| Record type | Host/name | Value/target |
| --- | --- | --- |
| `CNAME` | `qmm.labs.stonybrook.edu` | `<GitHub-owner-or-organization>.github.io` |

Important: the CNAME target should be the GitHub Pages default domain only, such as `USERNAME.github.io` or `ORGANIZATION.github.io`. Do **not** include the repository name in the CNAME target.

## If an IP address is required instead

GitHub documents A records for apex/root domains, not as the preferred setup for subdomains. If campus DNS policy requires IP addresses anyway, GitHub's current Pages IPv4 addresses are:

```text
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Optional IPv6 addresses are:

```text
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

## GitHub repository status

The GitHub Pages custom domain has been set to:

```text
qmm.labs.stonybrook.edu
```

The website repository is configured to deploy through GitHub Pages using GitHub Actions, and the site build includes the custom domain value.

## Verification after DNS is updated

After DNS propagation, verify the record with:

```bash
dig qmm.labs.stonybrook.edu +nostats +nocomments +nocmd
```

Expected result for the recommended setup: the output should show a CNAME chain from `qmm.labs.stonybrook.edu` to `<GitHub-owner-or-organization>.github.io` and then to GitHub Pages infrastructure.

DNS changes can take up to 24 hours to propagate. Once GitHub detects the DNS configuration, HTTPS should be enabled/enforced in the repository's GitHub Pages settings.

## Source

GitHub documentation: Managing a custom domain for your GitHub Pages site  
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
