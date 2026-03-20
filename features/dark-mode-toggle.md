# Feature: Dark Mode Toggle

## What

Add a dark mode toggle to the site. Users should be able to switch between light and dark themes from the header.

## Why

Dark mode is table stakes for a modern product site. Users expect it, and it signals that we care about the details.

## Behavior

- Toggle lives in the nav bar (right side, before "Get Started")
- Always visible, including on mobile
- Sun/moon icon to indicate current mode
- Switches the entire page — background, text, cards, everything
- Smooth transition, not a hard cut
- Remembers the user's choice across visits
- If the user hasn't chosen yet, match their OS setting
- No flash of the wrong theme on page load
- Logo should look right in both modes — a dark variant exists in the project

## Acceptance Criteria

- [ ] Toggle visible on mobile and desktop
- [ ] Clicking toggles between light and dark
- [ ] Page reload preserves the choice
- [ ] First visit respects OS preference
- [ ] No flash of wrong theme on load
- [ ] Meets WCAG 2.1 AA contrast and labeling
