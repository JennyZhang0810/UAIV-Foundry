# Deploying the UAIV-Foundry Project Page

This guide deploys the UAIV-Foundry project page to the existing GitHub repository:

```text
https://github.com/JennyZhang0810/UAIV-Foundry
```

The goal is to publish a clean project page first, without uploading the full internal engineering workspace.

## Files to Upload

Upload only these files at the repository root:

```text
index.html
README.md
DEPLOYMENT.md
.nojekyll
```

Do not upload the full local UAIV-Foundry workspace yet.

## Recommended Repository Structure for Now

The GitHub repository should initially look like:

```text
UAIV-Foundry/
├── index.html
├── README.md
├── DEPLOYMENT.md
└── .nojekyll
```

This keeps the public page clean while the full Foundry engineering repository is still evolving.

## Local Upload Steps

Copy the three files from:

```text
UAIV-Foundry/docs/io_site_package/
```

to a clean local folder, for example:

```text
D:\UAIV-Foundry-page
```

Then run:

```bash
cd /d D:\UAIV-Foundry-page

git init
git branch -M main
git add .
git commit -m "Initial UAIV-Foundry project page"
git remote add origin https://github.com/JennyZhang0810/UAIV-Foundry.git
git push -u origin main
```

If the remote repository already has files, run:

```bash
git pull --rebase origin main
git push -u origin main
```

If there are conflicts, stop and resolve them before pushing.

## Enable GitHub Pages

In the GitHub repository:

```text
Settings -> Pages
```

Use:

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

After GitHub finishes deployment, the page should be available at:

```text
https://JennyZhang0810.github.io/UAIV-Foundry/
```

## How to Update the Page Later

When `index.html` changes:

```bash
git status
git add index.html
git commit -m "Update UAIV-Foundry project page"
git push
```

When README or this deployment guide changes:

```bash
git add README.md DEPLOYMENT.md
git commit -m "Update UAIV-Foundry project page docs"
git push
```

## Release Boundary

The current page may say:

```text
pre-release engineering status
Golden/full annotation pending
release pending
benchmark dry-run ready
```

The current page must not say:

```text
UAIV-Real has been publicly released
Final QA passed
Real benchmark results are available
All annotations are reviewed
```

## Future Full Repository Release

After the Foundry engineering structure stabilizes, the full repository can be added progressively:

```text
awesome/
pipelines/
qa/
dashboard/
benchmark_runner/
datasets/
docs/
```

Before that step, internal logs, raw data, annotation exports, and private planning files should remain outside the public GitHub repository.
