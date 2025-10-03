# AI Instructions for NoobTaco's Midnight Testing

This file provides guidelines and context for AI tools and contributors working on this repository. Update and expand these instructions as your testing and documentation needs evolve.

---

## Purpose
- Assist with tracking, documenting, and summarizing addon and game feature testing for the WoW Midnight expansion.
- Help organize findings for the GitHub Wiki and other documentation outputs.

## General Guidelines
- Use clear, concise language in all documentation and summaries.
- When updating checklists, always use checkboxes and add notes for context.
- For compatibility issues, specify the addon, the problem, and any workaround or solution found.
- When documenting new features (e.g., Housing), include screenshots, links, and step-by-step test cases where possible.
- Prioritize high-impact or widely-used addons and features for testing and documentation.

## Wiki Preparation
- Structure findings by feature, addon category, or gameplay system for easy navigation.
- Use tables, checklists, and images to make information accessible.
- Summarize critical issues and solutions in a dedicated section.

## Collaboration
- Encourage contributors to add their own findings, notes, and screenshots.
- Use pull requests for major changes or new documentation sections.
- Keep this file updated as the project evolves.

## Test Case Creation Guidelines
- Assign a unique test case number (e.g., TC-001) to each new test case file.
- Place all test case files in the `test-cases/` directory.
- Link each test case from the main tracker checklist for easy navigation.
- Use a clear, consistent template: include objective, prerequisites, steps, expected/actual results, status, notes, date, and tester.
- Update the main tracker to reference or link the new test case.

## Addon Compatibility Tracker Guidelines
- When a new addon is to be tracked, add it to `addon-compatibility-tracker.md` in the appropriate section (or create a new section if needed).
- Use the standard checklist format: `[ ] <Addon Name> - [ ] Works / [ ] Workaround / [ ] Will be later / [ ] Not working`.
- Include space for status, notes, and last tested date for each addon.
- If the addon is high priority, add it to the High Priority Addons list as well.
- Keep the alphabetical and category order for easy navigation.

---

*Last updated: October 3, 2025*