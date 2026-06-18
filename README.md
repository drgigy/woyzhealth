# WOYZ Health website

Static website for `woyz.health`, ready for GitHub Pages.

## Files

- `index.html`: homepage
- `woyz-story.html`: Our Story page
- `admin.html`: private Firebase login page for demo requests
- `CNAME`: GitHub Pages custom domain
- `firestore-rules.txt`: Firestore rules to copy into Firebase

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

## Firebase Demo Requests

The Book a Demo form saves submissions into this Firestore collection:

- `demoRequests`

The admin page is available at:

- `https://woyz.health/admin.html`

Before testing, paste the rules from `firestore-rules.txt` into **Firebase > Firestore Database > Rules** and publish. The admin email is set to `drgigy@gmail.com`.
