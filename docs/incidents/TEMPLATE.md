# Incident N: <one-line title, e.g. "Silver job double-counts late rentals">

**Job:** `<job name>` · **Error class:** code / data / streaming / duplicates / silent logic · **Severity:** job failed / wrong numbers

## What I saw
The first signal: the failed run, the error message (first lines only), or the number that looked wrong. Screenshot in `../images/` if useful.

## How I found the cause
The steps that narrowed it down: what I checked, what I ruled out, and the query or log line that proved it.

## Root cause
One or two sentences.

## The fix
```python
# before
...
# after
...
```
Why this change, and why not the obvious alternative.

## Evidence
The run that went green, and a reconciliation number (row count, sum or duplicate check) showing the output is now right.

## What would catch it earlier
A test, constraint, expectation or alert that would have flagged this before anyone looked.
