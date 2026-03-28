# Child Downstairs (小朋友下樓梯) Implementation Plan

Create a modern, responsive web-based "Child Downstairs" game using HTML, CSS, and Vanilla JavaScript. The game will focus on survival by descending through various platforms while avoiding obstacles.

## User Review Required

> [!IMPORTANT]
> The initial version will use colored blocks for the player and platforms as requested. We can replace these with assets later.
> Please confirm if you want any specific scoring mechanics (e.g., items, combo points).

## Proposed Changes

### Core Game Engine

#### [NEW] [game.js](file:///c:/Users/Fongpei/Documents/code/child_downstair/game.js)
- Game loop using `requestAnimationFrame`.
- Physics engine (gravity, collisions, friction).
- Platform generation logic (randomized but balanced).
- Player controller (keyboard and touch support).
- State management (Start, Playing, Game Over).

### Styling and Layout

#### [NEW] [style.css](file:///c:/Users/Fongpei/Documents/code/child_downstair/style.css)
- Dark-themed design with neon accents.
- Responsive canvas centering.
- Typography using Google Fonts (Inter/Orbitron).
- UI components (Score overlay, Game Over screen).

### Entry Point

#### [NEW] [index.html](file:///c:/Users/Fongpei/Documents/code/child_downstair/index.html)
- Main game container and `<canvas>` element.
- Meta tags for SEO and mobile responsiveness.

## Open Questions

- Should the game speed increase over time?
- Do you have a preference for the player movement speed or gravity strength?

## Verification Plan

### Automated Tests
- N/A for this simple JS game, but will use manual browser testing.

### Manual Verification
1.  **Start Screen**: Verify the game starts correctly on click/keypress.
2.  **Movement**: Ensure the player moves left/right and reacts to gravity.
3.  **Collisions**: Check landing on different platforms (Normal, Moving, Spikes).
4.  **Game Over**: Test falling off or hitting top spikes.
5.  **Score**: Verify score increases as platforms pass.
6.  **Responsiveness**: Check performance on different window sizes.
