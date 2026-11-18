# Weekly management reporting

**Status:** Working Make.com workflow, run manually. Tested November 6, 2026 with fictional tasks.

## Problem
Managers need a consistent view of completed work, open items, overdue tasks, and missing ownership.

## Workflow
Task JSON → parsed records → calculated totals → AI summary → report for human review.

## Observed tests
- Six-task sample: 6 total, 2 completed, 4 open; inspected summary identified the correct overdue items.
- Empty task array: zero counts and an explicit no-records summary.

## Design choices
Counts are calculated before the AI writes the narrative. The summary must not invent progress or explanations for delays.

## Scope
Sample inputs and execution-history output. Live source connections, saved reports, and automatic schedules are future work. Built with AI assistance.


