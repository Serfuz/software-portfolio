# YATZY - Web-Based Local Multiplayer Game

## Overview
YATZY is a full-stack web application developed as part of the University of Stavanger course Webprogramming (DAT310). Built by a two-person team and awarded grade A, the project delivers a local hot-seat Yatzy experience for 2-4 players with authentication, saved games, and highscores.

The solution combines browser-side game logic with server-side persistence so users can continue games across sessions and manage their saved progress when logged in.

## Technologies
- Python
- Flask
- JavaScript (vanilla)
- HTML (Jinja templates)
- CSS
- SQLite
- REST-style JSON API endpoints
- Session cookies
- Werkzeug password hashing

## Team Size
2 computer engineering students.

## Key Features
- Login and registration with client-side and server-side validation.
- Secure password hashing and session-based authentication.
- Browser-based Yatzy gameplay with dice rolling and scoring logic.
- New game flow for 2-4 players.
- Save, load, update, and delete game saves for authenticated users.
- Highscore table with automatic updates when games are completed.
- Responsive layout for desktop and smaller screens.

## My Contributions
- Built and iterated the Flask backend, including routes for authentication, session lookup, highscores, and full save-game lifecycle (create/read/update/delete).
- Implemented server-side validation for login and registration, including password policy, email format checks, and structured HTTP status responses.
- Developed the SQLite data access layer, including user handling, game-save persistence, highscore updates, and database initialization with seed data.
- Implemented password hashing/verification with Werkzeug and enforced session-based access control for protected operations.
- Integrated frontend and backend flows with asynchronous API calls, form UX validation, my-games listing/sorting/open/delete actions, and highscore rendering.
- Contributed to gameplay persistence and board-state handling, including cookie-based resume behavior.
- Maintained and improved project documentation and testing guidance.

## What I Learned
- End-to-end design and implementation of a Flask + SQLite web application.
- Practical API design using REST-style routes, JSON contracts, and clear HTTP status semantics.
- Applied authentication and authorization patterns using hashed passwords and validated user sessions.
- Trade-offs between client-side state (cookies) and server-side persistence (database saves) in real user flows.
- Debugging and iterative delivery across backend logic, frontend behavior, and data model changes in a team setting.
- Better collaboration habits through consistent Git commits and living project documentation.

## Architecture
- Backend built with Flask for routing, validation, authentication, and API responses.
- Data layer separated into dedicated SQLite access functions for clear CRUD responsibilities.
- Frontend separated between interface/API communication logic and gameboard gameplay logic.
- Template-driven UI structure with reusable layout components.
