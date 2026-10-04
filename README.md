# B. Veerabhadrudu — portfolio

A small static portfolio for GitHub Pages. The deployment repository is `veera-1729/veera-1729.github.io`; the source also lives in this workspace under `portfolio/`.

## Publish an update from this workspace

From the root of `backend-prep-lab`, split the portfolio directory into a commit at the root of the publishing repository and push it to `main`:

```powershell
$portfolioCommit = git subtree split --prefix=portfolio HEAD
git push https://github.com/veera-1729/veera-1729.github.io.git "${portfolioCommit}:main"
```

The GitHub Actions workflow deploys the files to `https://veera-1729.github.io/` after a push to `main`.
