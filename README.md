# GitHub Pages Deployment Workflow

This project demonstrates how to set up a simple GitHub Actions workflow to automatically deploy a static website to GitHub Pages.

## Overview

The goal of this project is to help you learn the concepts of Continuous Integration and Continuous Deployment (CI/CD) using GitHub Actions. When you make changes to the `index.html` file and push them to the main branch, the workflow automatically deploys the updated website to GitHub Pages.

## Project Structure

```
gh-deployment-workflow/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow
├── index.html                  # Simple static website
└── README.md                   # Project documentation
```

## How It Works

1. **Trigger**: The workflow is triggered when changes are pushed to the `main` branch that affect the `index.html` file
2. **Deployment**: The workflow automatically deploys the website to GitHub Pages
3. **Access**: The deployed website is accessible at `https://<username>.github.io/gh-deployment-workflow/`

## GitHub Actions Workflow

The workflow (`.github/workflows/deploy.yml`) includes:

- **Trigger**: Only runs when `index.html` is modified on the main branch
- **Permissions**: Configured for GitHub Pages deployment
- **Steps**:
  - Checkout the repository
  - Setup GitHub Pages
  - Upload the website files as artifacts
  - Deploy to GitHub Pages

## Getting Started

1. Fork or clone this repository
2. Enable GitHub Pages in your repository settings
3. Make changes to `index.html`
4. Push changes to the main branch
5. The workflow will automatically deploy your changes

## Features

- ✅ Automatic deployment on `index.html` changes
- ✅ GitHub Pages integration
- ✅ Modern GitHub Actions syntax
- ✅ Proper permissions and security
- ✅ Concurrent deployment handling

## Learning Outcomes

After completing this project, you'll understand:

- GitHub Actions workflow syntax
- GitHub Pages deployment
- Continuous Integration and Continuous Deployment (CI/CD)
- Repository permissions and security
- Static website hosting

## Next Steps

For advanced learning, consider:
- Using static site generators (Hugo, Jekyll, Astro)
- Adding build steps and optimization
- Implementing testing before deployment
- Setting up custom domains
