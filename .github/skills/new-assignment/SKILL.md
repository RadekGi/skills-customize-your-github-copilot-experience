---
name: new-assignment
description: Create a new programming homework assignment for Mergington High School students. Use this skill whenever the user wants to create, add, scaffold, or generate a new assignment, exercise, or homework, even if they don't use the word "assignment" explicitly.
---

# Create New Programming Assignment

Assignments live in `assignments/<id>/`, and the website reads `config.json` to display them. Follow these steps to create both.

## Step 1: Gather Requirements

If the user hasn't specified, ask what programming concept the assignment should cover.

> Read `references/assignment-guide.md` for guidance on difficulty, scope, and when to include starter code.

## Step 2: Create the Assignment

1. Create `assignments/<kebab-case-id>/README.md` following `../../../templates/assignment-template.md`.
2. Optionally add starter code or data files to the same directory.

## Step 3: Register with the Website

Use the bundled scripts. Do not edit `config.json` manually.

**Register the assignment:**

```bash
node .github/skills/new-assignment/scripts/update-config.js <id> "<title>"