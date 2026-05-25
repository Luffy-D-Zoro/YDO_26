<!-- 
  PR TEMPLATE — READ BEFORE FILLING OUT
  ======================================
  This file contains comment blocks (like this one) with instructions for each section.
  Comments are wrapped in <!-- --> 
<!--
  When you're done, remove all comments between <!-- and -->.


## Summary
<!-- 
  What does this PR do and why?
  - One or two sentences describing the change and the motivation behind it.
  - Link the issue: "Fixes #123" or "Part of #123" (GitHub will auto-close the issue on merge if you use "Fixes").
  - If it's a non-obvious approach, briefly say why you went this way over alternatives.
  Example: "Fixes #42. Replaces the inline sort with a stable comparator to fix ordering on Safari."
-->

## Reviewer Guidance
<!-- 
  Help the reviewer spend their time in the right places.
  - Call out files or functions that are the core of the change vs. boilerplate.
  - Flag anything that's a deliberate tradeoff or might look wrong at first glance.
  - If the diff is large, suggest a reading order.
  Example: "Start with `src/utils/sort.js`: everything else follows from that change."
  Delete this section entirely if the change is small and self-evident.
-->

## Essential Checklist
- [ ] The PR title starts with `Fix #bugnum: `, followed by a short, clear summary of the changes. (If this PR fixes part of an issue, prefix the title with `Fix part of #bugnum: ...`.)
- [ ] "Allow edits from maintainers" is checked. ([Instructions](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork))
- [ ] The PR is made from a branch that's not called `main` or `master`.

## Proof of Work
<!-- 
  Show that the change works.
  - Screenshots or screen recordings for UI changes.
  - Terminal output or logs for backend/CLI changes.
  - "Tested manually by..." is fine for small fixes if there's nothing visual to show.
  If your change is covered entirely by automated tests, note that here and delete the rest.
-->

## AI Usage Disclosure
<!-- 
  Disclose if and how AI tools were used in this PR.
  - This includes code generation, writing commit messages, drafting this description, etc.
  - You don't need to list every autocomplete suggestion, focus on substantial use.
  - If no AI tools were used, write "None." and leave it at that.
  Example: "Used Copilot to scaffold the test file; reviewed and modified all suggestions."
-->
