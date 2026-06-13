# WOYZ Health website

Static website for `woyz.health`, ready for GitHub Pages.

## Files

- `index.html`: homepage
- `woyz-story.html`: Our Story page
- `CNAME`: GitHub Pages custom domain

## Publish with GitHub Pages

1. Create a GitHub repository and upload all files in this folder.
2. In the repository, open **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then save.
5. Under **Custom domain**, enter `woyz.health` and save.
6. After DNS verification succeeds, enable **Enforce HTTPS**.

## GoDaddy DNS

Set these records for the root domain:

| Type | Name | Value |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |

Remove conflicting `A`, `AAAA`, or forwarding records for `@`. DNS changes can take time to propagate.
