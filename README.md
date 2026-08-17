What NeuroLab Is

NeuroLab is a browser-based puzzle game built around a single core mechanic: guiding a green "neuro-ball" through a maze. The site presents itself as a small, self-contained web game (hosted on Vercel) rather than a complex application — it's a single-page interface with a title screen, gameplay screen, pause overlay, and level-complete screen.

How It Works

Core mechanic — "slide until you hit a wall": Unlike a typical maze game where you move one tile at a time, the ball here moves continuously in whichever direction you choose until it collides with a wall. This is often called a "sliding maze" or "ricochet" mechanic (similar in spirit to games like ricochet robots), which makes the puzzle about planning a sequence of directional slides rather than just tracing a path.

Controls:

Arrow keys to set direction
Swipe gestures (for touch/mobile devices)
Enter or a swipe starts the level
Escape pauses and resumes the game

Content structure:

The game consists of 30 levels, each a distinct maze rendered as SVG graphics (dense, intricate wall layouts).
Levels must be completed in order — finishing one unlocks the next.
The interface tracks two stats per level: the current level number and the number of moves used, encouraging players to solve each maze efficiently rather than just eventually.

Progression and saving:

Progress is saved locally in the browser (likely via localStorage), so players can close the tab and resume later without an account or login.

UI states:

A pause menu appears on Escape, with options to Continue, Restart, or return to the Menu.
A level-complete screen appears on finishing a maze ("neuro-route stabilized" is the flavor text), showing the level and move count, with options to advance to the Next level, Retry, or go to the Menu.
