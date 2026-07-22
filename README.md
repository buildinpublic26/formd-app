# Formd — AI Gym Tracker

Formd is a workout tracker built for lifters, exercise ethusiasts and Hyrox athletes. Log sessions, build training programmes, track body metrics, and record milestones — all synced to your account via Supabase, with full offline support. This README is a complete tour of what the app can do today.

---

## Getting started

- **Sign up** with a display name, email, and password (min. 6 characters).
- **Log in** any time — your data follows you across devices since everything lives in your account, not on one phone or browser.
- **Forgot password?** Use the link on the login screen to get a reset email.
- Formd works **offline** — log a session with no signal and it queues locally, then syncs automatically the next time you're online (you'll see an orange "Offline" badge in the top bar while disconnected).

---

## Log — recording a workout

This is the home tab, and where most sessions start.

- **Workout type** — Push/Pull/Leg Day, Upper/Lower/Full Body, Cardio, Core, Hyrox Training, Hyrox Race Simulation, or Custom.
- **Date, weight unit (kg/lbs), and session notes.**
- **Add Exercise:**
  - Type an exercise name — autocomplete searches Formd's built-in list of 130+ exercises across every muscle group, plus **any exercise name you've personally used before** (see "Your own exercise names" below).
  - Choose a tracking type: **Strength** (reps/weight/unit/notes), **Cardio/Distance** (distance/unit/time), or **Hyrox** (distance-or-reps/load/time/notes).
  - Build your sets, then tap **"Add to session."**
  - Added exercises appear below with every field inline-editable, and a **"+ Set"** button to add another set on the fly.
- **Formd remembers your last numbers.** Pick an exercise you've logged before (or type its name and tap away from the field) and the set builder pre-fills with the reps, weight, and notes from the last time you did it — no retyping. A small tip banner briefly shows what was pulled in. You can edit anything before saving.
- **Rest timer** — 60s / 90s / 2m buttons with a live countdown and a phone vibration when time's up.
- **Save workout session** once you're done — this is what actually commits everything to your account.

### Hyrox Quick Log
Switch the workout type to **Hyrox Training** or **Hyrox Race Simulation** and a station grid appears — tap any of the 8 official Hyrox stations (SkiErg, Sled Push/Pull, Burpee Broad Jumps, Rowing, Farmers Carry, Sandbag Lunges, Wall Balls, plus the 1km runs) to jump straight into logging it.

---

## My Plan — training programmes

Build a repeatable training schedule instead of starting from scratch every session.

- **Create a programme** — name it, add an optional description, and pick which days of the week you train.
- **Build each training day** — set the workout type and add exercises with target sets/reps/weight (or distance/load/time for Hyrox and cardio days).
  - **Copy day** — reuse another day's exercises as a starting point instead of rebuilding from scratch.
  - **Hyrox Race Simulation** auto-populates the full official 16-part race order (8 runs + 8 stations). **Hyrox Training** auto-populates a scaled interval template. Both are only applied if the day is empty — Formd never overwrites exercises you've already added.
- **Load a day straight into Log** — tap **"Log this"** on any plan day, or use **"Load from My Plan"** on the Log tab. Formd checks your real logged history for each exercise first and pre-fills your actual last performance; only exercises you've never logged before fall back to the plan's saved target numbers. A tip shows how many exercises came from history vs. the plan.
- **Add extra exercises into a plan day while logging** — if you loaded today's session from a My Plan day and want to bolt on something extra, a checkbox appears under Add Exercise: *"Also add this exercise to My Plan: {day}."* Tick it before adding, and that exercise is saved into the plan going forward — additive only, nothing existing is ever removed or overwritten.
- Plans sync across every device via your account — no local-only storage.

---

## Your own exercise names

Gyms and coaches don't always call things the same thing. Type any exercise name that isn't already in Formd's built-in list, and the moment you add it to a session, Formd quietly remembers it — no extra setup. From then on it shows up in autocomplete everywhere (Log and My Plan) across all your devices.

---

## History

- Every saved session as an expandable card — tap to see each exercise and every set.
- **Edit a session** — change the workout type, date, notes, or any individual set's reps/weight/unit/notes, right from History.
- **Delete a session** if you logged something by mistake.

---

## Body Metrics

Track your physical stats over time:

- Weight (kg), body fat %, visceral fat score, skeletal muscle %, body water %, plus free-text notes (e.g. "morning weigh-in").
- **Latest Reading** card gives you an at-a-glance snapshot; **Recent History** lists your last 20 entries.

---

## Goals (Milestones)

Log the wins as they happen:

- Personal Best, Strength Milestone, Hyrox PB, Weight Goal, Consistency Win, or a General Note.
- Add a title and details, and it's saved with the date automatically. Delete any milestone you no longer want tracked.

---

## Stats

An at-a-glance dashboard:

- **Total sessions, sessions this week, current day streak, and Hyrox session count.**
- **Personal Bests** — heaviest weight logged per exercise.
- **Most logged exercises** — frequency bars showing what you train most.
- **Session breakdown** — how your workout types are distributed.

---

## Data safety

Everything you log lives in your account in the cloud (Supabase), not just on one device — sign in anywhere and it's all there. Offline logging is queued locally and synced automatically once you're back online, so you never lose a session because of a bad signal at the gym.

---

## A quick note on the AI Plan tab

There's an AI Plan Builder tab in the app that's currently disabled for the MVP — it'll generate a personalised training plan from your goals, stats, and constraints in a future update.
