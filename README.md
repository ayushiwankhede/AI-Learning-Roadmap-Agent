# AI Learning Roadmap Agent

An AI-powered personalized learning-roadmap generator built with **n8n**, **Google Gemini**, and **Gmail**.

## What it does
1. Collects a learner's name, email address, target skill, and learning pace through an n8n form.
2. Sends the learner's details to Google Gemini, which generates a detailed HTML learning roadmap.
3. Emails the generated roadmap to the learner through Gmail.

The roadmap is designed to include core sub-skills, learning stages, practice-hour estimates, a 30-day kickstart plan, tools, resources, milestones, career use cases, potential earning paths, and first steps.

## Workflow
`Form submission → Google Gemini → Gmail`

## Repository contents
- `workflow.json` — sanitized n8n workflow export.
- `sample-roadmap.md` — an illustrative sample roadmap for a beginner learning Python. It is not an output captured from a live workflow run.
- `screenshots/` — optional screenshots can be added here later.

## Requirements
- An n8n instance
- Google Gemini API credentials configured in n8n
- Gmail OAuth2 credentials configured in n8n

## Import and configure
1. Import `workflow.json` into your n8n instance.
2. Configure your own Google Gemini credentials in the AI node.
3. Configure your own Gmail OAuth2 credentials in the email node.
4. Review the form fields and prompt.
5. Test using an email address you control before enabling the workflow.

This repository does not include API keys, OAuth tokens, or working credentials. You must configure your own integrations.

## Current status
Shared as a portfolio project. The original n8n cloud trial expired, so this repository does not claim that a hosted instance is currently running.

## Safety and limitations
- Never commit API keys, OAuth tokens, passwords, or private user submissions.
- Review generated HTML before sending it to users.
- AI-generated learning timelines, job-readiness estimates, and income figures are estimates, not guarantees.

## Technologies
- n8n workflow automation
- Google Gemini
- Gmail
- HTML email generation
