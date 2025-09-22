# CodeReaper

Centralized security scanner.  
Runs automated scans across all public repos, aggregates vulnerabilities, secrets, dependency and supply chain issues into a master report.  
Fast, simple, ruthless.
Catching security issues before they become a headache.

## Requirements to setup

The automation will create labels in your repo if they are not already present:

- security
- critical
- high-priority
- medium-priority
- low-priority
- immediate-action
- action-needed
- review-needed
- routine-scan
- good-status

You don't need to leverage some of the aggregated scans but doing so is recommended. In order to have the full breadth of scans, you'll need:

- `SNYK_TOKEN`:Snyk token via the cli key found in your https://app.snyk.io/ account
- `OSS_INDEX_USERNAME`: owasp username in the account found here: https://ossindex.sonatype.org/user/settings
- `OSS_INDEX_TOKEN`: owasp token https://ossindex.sonatype.org/doc/auth-required
