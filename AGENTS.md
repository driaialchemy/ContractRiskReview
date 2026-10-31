# AGENTS.md

## Purpose

Asynchronous CUAD contract-risk pipeline. It extracts clauses, compares them to a legal playbook, and writes audit reports.

## Setup

pip install -r requirements.txt

Set the CUAD zip path with the environment variable documented in README.md.

## Tests

pytest tests/ -q

## Sensitive areas

`.env` files, `data/logs/`, contract inputs, `data/playbook.json`, and `governance/specs/`.

## Approval gates

Human approval is required before dependency changes, external-call changes, deploy or container config, secrets, and AI-provider or database config.

## Verification

Run `pytest tests/ -q` after every change.
