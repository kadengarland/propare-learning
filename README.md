# Propare Learning OS

A single-file local learning system built to take over full backend engineering
ownership of a venture-backed startup by a hard deadline.

## Background

Propare is a two-sided coaching marketplace I co-founded connecting athletes
with verified coaches through live 1:1 sessions and video analysis. As CPO/COO,
I needed to become technically self-sufficient on the backend before our lead
developer departs. This app is the system I built to get there.

## Overview

124 tasks across 6 progressive stages — Reader through Technical Founder,
Levels 1 to 30. Built entirely in one HTML file with no dependencies beyond
Google Fonts. Open it in a browser and all state saves automatically to
localStorage.

## Tabs

**Today**
Daily task queue with time filters (30 min, 1-2 hrs, 3-4 hrs, Full day).
Shows a typewriter animation on the day label each time it changes. Includes
a collapsible Behind Schedule section that groups overdue tasks by day with
urgency styling. No Help Mode toggle hides all "Why this matters" sections
to force recall from memory. Practice Scenario button launches a random
scenario directly from Today.

**All Tasks**
Full 124-task list with live search and track filters: Code Reading, Building,
Debugging, Azure, Developer Sessions, Generation, and Critical. Critical tasks
have a separate filter and badge treatment.

**Retention Checks**
Spaced repetition system. Tasks resurface on a 3-day then 7-day interval
before being marked owned. Retention streak counter tracks consecutive
successful check-ins.

**Notes**
Freeform notes tab tied to localStorage.

**Failure Log**
Tracks tasks where recall failed. Badge count on the nav tab shows open
failures at a glance.

**Developer Prep**
Dedicated tab for questions and knowledge gaps to surface before the
engineering handoff.

**Quick Reference**
Cheat sheet for key backend patterns, commands, and concepts.

**Progress**
Four dashboard metric cards (tasks done, XP, streak, stage progress) with
odometer animations on value changes. Achievements grid, competency
breakdown, and a readiness checklist for the handoff deadline.

**Scenarios**
Real-world engineering situations to work through. Scored and filterable
by track. Results logged per scenario.

## XP and Progression System

Each completed task awards XP. XP fills a progress bar toward the next
level. Levels 1 to 30 map across six named stages. Level-up triggers a
full-screen banner. Achievements unlock at milestones and surface as
toast notifications. Streak tracking awards a distinct amber glow on the
metric card when active.

## Visual Design

"Mission Control meets Bloomberg Terminal" aesthetic. Deep near-black
backgrounds with lime green `#A4DE02` as the primary accent. Noise texture
and subtle scanline overlay on the body. Ambient floating code symbols drift
through the left and right margins only — no cursor interaction — keeping
the content area clean. Aurora spotlight effect on task cards tracks the
mouse position with a radial gradient. Tab transitions animate in and out.
Nav underline slides between active tabs.

## Stack

- Single HTML file — no build step, no dependencies
- Space Grotesk, JetBrains Mono, Geist, Geist Mono via Google Fonts
- All state persisted to localStorage
- Fully mobile-optimized — touch devices get active states instead of hover,
  aurora spotlight disabled on touch
- Animation pauses automatically when the browser tab is not visible

## Scope

Covers the full Propare tech stack across six learning tracks: Code Reading,
Building, Debugging, Azure, Developer Sessions, and Generation. Primary focus
is the FastAPI/Python backend, PostgreSQL, Docker, and Azure infrastructure.
Also includes Next.js frontend reading -- auth state, proxy chain, deployment
pipeline -- and Phase 4 builds that extend into full-stack features.

## Repo

[github.com/kadengarland/propare-learning](https://github.com/kadengarland/propare-learning)
