---
name: frontend-implementation
description: Use when Codex is building, modifying, or polishing a web frontend, including React/Vite apps, static HTML/CSS/JS pages, dashboards, forms, responsive layouts, and browser-based tools, and should implement the UI using existing project conventions then verify it in a real browser.
---

# Frontend Implementation

Use this skill to turn frontend requests into working browser-visible UI with a tight implementation and verification loop.

## Workflow

1. Inspect the project before editing.
   - Read package files, app entrypoints, routing, component folders, styling setup, and nearby examples.
   - Identify the framework, build command, dev server command, design system, icon library, and test tooling.
   - Prefer existing components, tokens, utilities, and layout patterns over new abstractions.

2. Define the user-facing behavior.
   - Translate the request into concrete screens, states, controls, and interactions.
   - Include empty, loading, error, disabled, hover/focus, and mobile states when they are relevant.
   - Avoid creating a marketing landing page unless the user specifically asked for one.

3. Implement in small, cohesive edits.
   - Keep changes close to the feature boundary.
   - Use semantic HTML, accessible labels, keyboard-friendly controls, and responsive constraints.
   - Use the existing icon library when available. If the project uses Lucide, prefer Lucide icons for common actions.
   - Do not add ornamental gradients, floating blobs, or unrelated decorative UI.

4. Verify with the actual app.
   - Run the project's formatter, typecheck, linter, and tests when available and proportionate.
   - Start the local dev server for apps that require one.
   - Open the page in a browser, inspect screenshots at desktop and mobile widths, and check for blank screens, console errors, clipped text, overlap, broken assets, and unusable controls.
   - Exercise the main interactions, not just initial render.

5. Report the result.
   - Summarize the files changed and the behavior delivered.
   - Include the local URL when a dev server is running.
   - State any verification command that could not be run.

## Visual Quality Rules

- Make the requested app or tool the first screen. Do not insert a generic hero or explanatory page before the useful experience.
- Keep operational interfaces dense, calm, and scan-friendly. Use cards only for repeated items, modals, and genuinely framed tools.
- Use stable dimensions for boards, toolbars, counters, tiles, and fixed-format controls so dynamic content does not shift the layout.
- Ensure text fits inside buttons, cards, sidebars, and compact panels across desktop and mobile.
- Avoid one-note color palettes. Use project tokens first; otherwise choose a restrained palette with sufficient contrast and more than one visual role.
- Never let UI text or controls overlap incoherently. Fix layout constraints before calling the work complete.

## Browser Verification Checklist

Use this checklist before final response:

- App/page loads without a blank screen.
- Console has no relevant runtime errors.
- Primary flow can be completed with mouse or keyboard.
- Desktop layout is correctly framed and not sparse by accident.
- Mobile layout does not clip, overlap, or hide essential controls.
- Images, icons, fonts, and canvases render as intended.
- Hover, focus, disabled, selected, empty, loading, and error states are handled when relevant.

## When Existing Instructions Conflict

Follow the user's explicit request and the repository's own instructions first. Use this skill as the frontend execution pattern around those constraints.
