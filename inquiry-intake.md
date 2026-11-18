# AI inquiry intake

**Status:** Working Make.com workflow, run manually. Tested November 6, 2026 with fictional inquiries.

## Problem
Incoming inquiries need classification and a useful first response while preserving human review.

## Workflow
Sample inquiry → AI classification and response draft → JSON parsing → review record.

## Observed tests
- Normal inquiry: inquiry_automation classification, needs_human_review status, populated draft.
- Instruction override requesting a customer database: suspicious classification, manual_review status, blank draft.

## Design choices
Drafting is separate from sending. Suspicious content is routed for review. No emails were sent.

## Scope
Embedded sample data and execution-history output. Live webhook input, persistent review queues, and duplicate protection are future work. Built with AI assistance.


