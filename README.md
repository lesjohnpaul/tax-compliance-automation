# Tax Compliance Automation

> Two weeks of manual compliance work became two clicks and under 5 minutes.

**Status:** In production · **Client:** 250K-member electric cooperative · **Role:** Solo engineer

**Stack:** `Process Automation` `PDF Generation` `Compliance` `MS SQL Server`

> [!NOTE]
> **Showcase repository.** The source code is private and belongs to the client. This repo documents the problem, the architecture, and the results. Screens show demo data. Full case study: https://lesjohnpauloliver.dev/work/tax-compliance-automation

## Summary

Regulatory tax compliance reporting that took the compliance team two weeks is now a two-click run that finishes in under 5 minutes.

## The problem

- Building the regulated reports took two weeks of manual work each cycle.
- Copying figures by hand into the reports risked transcription errors in filings.

## Problem → fix

### Building the regulated reports took two weeks of manual work every cycle.

A two-click run pulls the figures from MS SQL Server and generates the regulated PDFs in under 5 minutes.


### Copying figures by hand into the reports risked errors in the filings.

No one retypes a number. The data pull is read-only, and the same data always produces the same report, so a filing can be regenerated on demand.


## Approach

- Pull the figures straight from the billing database so no one retypes a number.
- Generate the regulated PDFs directly, so the output is the filing.

## What was built

- Two-click run that pulls the data from MS SQL Server
- Automatic generation of the regulated PDF reports
- No manual transcription step anywhere in the process

## Architecture

- The run reads the source figures directly from MS SQL Server.
- A generation step turns those figures into the regulated PDF reports.
- Staff start the whole process with two clicks; no figure is copied by hand in between.

## Engineering

- Removing manual transcription removes the main source of filing errors.
- The data pull is read-only, so producing a report cannot change the billing records.
- The same run produces the same report from the same data, so a filing can be regenerated on demand.

## Where AI does the work

Automation replaces the manual data pull and report building end to end.

## Outcome

- 2 weeks of manual work → under 5 minutes, two clicks.

---

Built by **[Les John Paul Oliver](https://lesjohnpauloliver.dev)**, AI Engineer in the Philippines: agentic AI, RAG, LLM evals, MCP, and business automation. [Case studies](https://lesjohnpauloliver.dev/#projects) · [Hire me](https://lesjohnpauloliver.dev/ai-engineer-philippines)
