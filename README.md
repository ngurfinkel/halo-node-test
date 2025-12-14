# auto-merge-middle-level

Test repository for auto-merge workflow validation - Level 2 (middle tier).

This repository demonstrates automatic PR creation and auto-merge functionality in a multi-tier setup.

## Purpose

- Contains `auto-merge-bottom-level` as a submodule in `lib/auto-merge-bottom-level`
- When the submodule is updated, this triggers a workflow that:
  1. Updates the submodule pointer in the parent repository (auto-merge-top-level)
  2. Creates an auto-PR with `(auto)` prefix
  3. Auto-merge is enabled automatically
  4. PR merges when all checks pass

## Part of Test Chain

auto-merge-bottom-level → **auto-merge-middle-level** → auto-merge-top-level

