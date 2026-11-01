
# Stellantis Vehicles Worker V2 — Peugeot OAuth Fixes

> Community fork with Peugeot authentication improvements, based on PR #3.

This repository is a fork of [Stellantis Vehicles Worker V2](https://github.com/andreadegiovine/homeassistant-stellantis-vehicles-worker-v2) by andreadegiovine.

It includes improvements to the MyPeugeot OAuth authentication process.

## What's different in this fork?

### Peugeot OAuth redirect and consent flow

Based on PR #3, this fork includes improvements to the Peugeot OAuth redirect and consent flow.

Related commit: `83f3675`

### Visible login field detection

An additional fix improves the detection of visible login fields during browser-based MyPeugeot authentication.

This helps handle login pages containing multiple input elements, including hidden fields.

Related commit: `d7b1df6`

## Installation

Clone the branch containing the Peugeot OAuth fixes:

```bash
git clone --branch fix-peugeot-oauth-pr3 https://github.com/lhplab/homeassistant-stellantis-vehicles-worker-v2.git
```

The Worker uses Python, FastAPI and Playwright/Chromium.

Use the Dockerfile and requirements provided in this repository to build the Docker image.

The Worker operates alongside the Stellantis Vehicles integration for Home Assistant.

## Compatibility

These changes target MyPeugeot OAuth authentication.

They have been tested in a Docker-based deployment. Compatibility with all Peugeot vehicles, Stellantis brands and authentication scenarios is not guaranteed.

## Credits

Original project: [andreadegiovine/homeassistant-stellantis-vehicles-worker-v2](https://github.com/andreadegiovine/homeassistant-stellantis-vehicles-worker-v2)

Peugeot OAuth improvements based on PR #3 (commit `83f3675`).

Additional visible login field detection fix (commit `d7b1df6`).

## AI Assistance Disclosure

Development, debugging and troubleshooting of the additional Peugeot authentication fix were carried out with assistance from OpenAI's ChatGPT.

The resulting changes were integrated and tested by the fork maintainer.

AI assistance does not imply endorsement by OpenAI.
