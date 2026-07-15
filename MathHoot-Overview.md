# MathHoot — Project Overview

*A self-contained, browser-based quiz game for mathematics*

**What it is.** MathHoot is a Kahoot-style quiz game built for mathematics. It runs in any web browser from a single file — nothing to install, and you can play without signing in. An optional free account syncs your content across devices.

**Setting up a quiz.** Before starting, a player picks:

- **Topics** (any of ten): Arithmetic, Fractions & Percents, Algebra, Powers & Roots, Geometry, Number Theory, Statistics, Sequences, Trigonometry, and Calculus.
- **Question types:** numerical, conceptual, and/or true/false.
- **Difficulty:** Easy through College, or Adaptive (auto-adjusts as you answer).
- **Length, pace, and scoring:** 5–20 questions, an optional timer, and time-based (Kahoot-style) or simple correct-count scoring.

The game then presents questions one at a time on color-coded answer tiles with a live countdown — each question labelled with its difficulty level, and quittable at any point — and ends with a results screen.

**What makes it different.** Questions are *generated*, not pulled from a fixed list — each topic has dozens of question forms with randomized numbers, so no two games are alike. Difficulty changes the *kind* of problem, spanning introductory arithmetic up to genuine university-level material (logarithms, matrices, complex numbers, vectors, infinite series, calculus, and more). A built-in **question catalog** shows how many templates exist for each topic and difficulty level — and any number can be tapped to view the templates themselves.

**Feedback that teaches.** The results screen includes a **report card** — the percentage correct in each subject area tested — and a question-by-question **review** where each item expands to a short explanation and a direct link to the relevant Khan Academy lesson (explanations for missed questions shown by default).

**Make and share your own.** Players can build custom question sets — typing questions in, or picking specific problems from MathHoot's own bank — then play them or **share** a set with anyone via a link or short code.

**AI Integration.** Describe a quiz in plain English and Claude (Anthropic's AI) writes the whole set — questions, four answer choices, the correct answer, and a short explanation for each — saved directly to your question sets to play solo or host live. Because MathHoot runs entirely in the browser, it uses your own Anthropic API key, stored only on your device.

**Accounts and live classroom games.** A free account (teacher or student) syncs sets, history, and preferences across devices — with email-based password reset — and student accounts get **personalized recommendations** — MathHoot tracks a student's accuracy by topic, flags weak areas to review, and builds a targeted practice set on request. A **teacher can host a live game** — a custom set or a generated quiz — and students join with a code on their own devices. The teacher drives it question by question, Kahoot-style, with a live leaderboard, all in real time and with no extra server.

**Accessible and multilingual.** An **Accessibility & language** panel adds high-contrast, larger-text, readable-spacing, and reduced-motion display modes, plus screen-reader labels on the questions and answers, and an interface language selector (English / Español). Choices are saved to your preferences.

**Technical note.** The whole app is a single ~2,000-line HTML file with no build step; its only external dependency is Firebase, used for the optional account sync and live games (offline, the single-player game runs fully local). It is published at **https://wmeleis.github.io/mathhoot/**. The question logic was verified by automatically generating over 100,000 sample questions with zero formatting errors, plus a manual check of the mathematics. This is an early working draft.
