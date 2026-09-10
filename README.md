# FOSSA CLI + GitHub Actions Technical Exercise

## Overview

You have **20 minutes** to integrate the FOSSA CLI into this sample repository using **GitHub Actions**.

The goal of this exercise is to demonstrate your ability to work with CI/CD, integrate a security/compliance tool into an existing development workflow, troubleshoot issues, and communicate your technical decisions.

## Objective

Create a GitHub Actions workflow that integrates the **FOSSA CLI** into this repository.

Your workflow should:

* Run automatically on **pull requests**
* Authenticate with FOSSA securely
* Execute a FOSSA analysis
* Fail the workflow appropriately when the FOSSA CLI reports a failure
* Produce useful output that allows someone reviewing the workflow to understand the scan results

## Requirements

### 1. GitHub Actions Workflow

Create a GitHub Actions workflow under:

```text
.github/workflows/
```

The workflow should:

* Trigger on pull requests
* Install or otherwise make the FOSSA CLI available to the runner
* Authenticate securely using a GitHub secret
* Run the FOSSA CLI against the repository
* Return an appropriate exit status so that GitHub Actions can determine whether the workflow passed or failed

**Do not commit credentials, API keys, or other secrets to the repository.**

### 2. Review the Results

After running the FOSSA analysis, review the results for:

* **Licensing issues**
* **Security/vulnerability issues**

You do not necessarily need to resolve every issue you find.

Instead, be prepared to explain:

* What issues you found
* Whether they appear legitimate
* What you would recommend doing about them
* Whether anything appears unexpected or potentially incorrect
* What additional information you would want from the customer if this were a real implementation

### 3. Explain Your Decisions

As you work through the exercise, explain your technical decisions.

Be prepared to discuss:

* Why you structured the GitHub Actions workflow the way you did
* How you handled authentication
* How the workflow determines success or failure
* Anything you would change for a production deployment
* Any assumptions you made
* Any issues or obstacles you encountered

## What We're Evaluating

We are primarily interested in **how you approach the problem**, not simply whether you produce a working YAML file.

We'll be looking at:

* GitHub Actions and CI/CD knowledge
* Ability to integrate a third-party CLI into a build pipeline
* Secure handling of credentials and secrets
* Familiarity with command-line tooling
* Troubleshooting and debugging approach
* Understanding of software composition analysis, licensing, and vulnerabilities
* Ability to distinguish product issues from configuration/environment issues
* Technical communication
* Ability to explain tradeoffs and assumptions
* Customer-oriented problem solving

## Time Limit

**20 minutes**

You may use documentation and other publicly available resources as you normally would when solving a real customer problem.

At the end of the exercise, please walk us through your implementation and explain your findings.
