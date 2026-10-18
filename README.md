"# To-Do App" 
# Larder

> A todo app that respects your attention.

**Larder** is a small, opinionated personal task app. It is not a project
manager, not a team workspace, and not a second brain. It is a place to
capture what you need to do, decide what actually matters today, and get
on with your day.

The name is deliberate: a larder is where you keep what you need, in
small quantities, within reach. That is the whole idea.

---

## The problem

Most todo apps fail in one of two directions:

1. **They become filing cabinets.** Projects, sub-projects, tags, custom
   fields, priorities, dependencies, boards, timelines. You spend more
   time organizing tasks than doing them.
2. **They become guilt machines.** Overdue badges, streaks, red
   counters, reminder spam. The app starts to feel like a disappointed
   manager.

Larder is an attempt to be neither. It assumes that:

- You have a small number of things that actually matter today.
- Most tasks do not need a due date, a priority, or a category.
- Capture should take seconds and require no decisions.
- A tool that nags you is a tool you eventually delete.

---

## What Larder is

Larder is a **personal task inbox** with four surfaces:

| Surface | What it holds |
|---|---|
| **Inbox** | Everything you captured but haven't decided about yet. |
| **Today** | A short, manually ordered list of what you intend to do today. |
| **Upcoming** | Tasks with a date, grouped by day. |
| **Lists** | Flat buckets like *Work*, *Home*, *Errands*. No nesting. |

Plus a few quiet utilities: search, an archive of completed tasks, data
export, and account deletion.

That's it. That is the whole product.

---

## The core loop

Larder is built around one loop, and everything in the app exists to
serve it:

1. **Capture.** Type a title. Press Enter. The task lands in the Inbox.
   Nothing else is required — no date, no list, no tag.
2. **Triage.** When you have a minute, open the Inbox and decide: keep
   it, schedule it for today, give it a date, move it to a list, or
   delete it. Triage is a separate activity from doing.
3. **Do.** Open Today. You see a short list you deliberately chose
   yourself. Work through it. Reorder it if you change your mind.
4. **Complete.** One click or keystroke. Undo is always available.

If a feature does not make one of those four steps faster, safer, or
calmer, it does not belong in Larder.

---

## Design principles

These are the rules the app is built against. They explain most of the
product decisions you'll notice while using it.

### 1. Capture is sacred
Adding a task takes one field and one action. Details are optional and
added later. Any friction at capture time is a bug.

### 2. One place for unsorted work
Everything you capture goes to the Inbox first. The Inbox is not a
backlog you are failing to clear — it is a queue you are allowed to
ignore until you triage.

### 3. Today is a commitment, not a dump
The Today view is intentionally small. You put tasks there by hand.
Nothing is auto-promoted into Today. The size of that list is a signal
you should not be able to fake.

### 4. Defaults should be quiet
No due date, no priority, no list, no tag by default. Most tasks do not
need metadata. If you want it, it is one click away — not forced on you
at creation.

### 5. No guilt mechanics
No streaks. No red badges. No "you have 47 overdue tasks." No
aggressive reminders. When a task slips, you reschedule it or drop it.
The app does not editorialize.

### 6. The app gets out of the way
Keyboard-first on desktop. Thumb-friendly on phone. Clear undo
everywhere. Loading states that don't lie. Nothing shakes or slides or
celebrates.

### 7. Your data is yours
Full export, in a format you can read, at any time. Full account
deletion, not a deactivation toggle. No lock-in, no dark patterns.

---

## What's included

- Fast capture from anywhere in the app
- Inbox, Today, Upcoming, and flat Lists
- Optional due dates and simple reminders
- Simple recurring tasks: daily, weekly, monthly — nothing more
- Manual ordering within Today
- Complete with undo
- Search across open and completed tasks
- Archive of completed tasks
- Full data export (JSON)
- Full account deletion
- Notifications that you can mute entirely, in one switch
- Keyboard-first interaction on desktop
- Responsive layout for phone and desktop
- Accessible by default: focus order, labels, contrast, screen-reader
  support

---

## What's deliberately excluded

This list is as important as the one above. Each item here has been
considered and rejected, not overlooked.

- **Team collaboration.** No comments, assignments, permissions, or
  shared workspaces.
- **Project management features.** No kanban boards, Gantt charts,
  dependencies, or portfolios.
- **Habits, streaks, gamification.** No XP, badges, or progress rings.
- **Rich task content.** No attachments, embeds, or rich text. A short
  notes field is enough.
- **Complex metadata.** No custom fields, no priority matrices, no deep
  tag hierarchies, no nesting.
- **A calendar.** A task can have a date. Larder will never become your
  calendar.
- **AI scheduling or chat assistants.** The core loop must be
  excellent before anything else is added on top.
- **Social features.** No feeds, no sharing, no public profiles.
- **Integration marketplaces.** No plugin systems, no automation
  builders.
- **Forced signup to try the app.** Account creation is required to
  persist data, not to understand what the product is.

If you're looking for any of the above, Larder is not for you — and
that is on purpose.

---

## Who it's for

Larder is for people who:

- Have tried heavier todo apps and spent more time configuring them than
  using them.
- Want a small, daily tool, not a second job.
- Are comfortable with the idea that a task list should be small.
- Care about owning their data.

It is probably **not** for people who:

- Need to coordinate tasks with other people.
- Manage large projects with many moving parts.
- Want a single app to replace their notes, calendar, wiki, and tasks.
- Enjoy dashboards.

---

## The reasoning behind some decisions

A few product decisions that are easy to question, and why they are the
way they are:

**Why an Inbox and not just a full task list?**
Because capture and triage are different cognitive activities. Mixing
them makes both worse. The Inbox gives you a place to dump without
deciding, and a separate moment to decide without scrambling to
remember things.

**Why manual ordering in Today?**
Because priority is not a number. It changes through the day. Manual
ordering lets you express what matters *right now* without pretending
you can rank 200 tasks consistently.

**Why no default due date?**
Because a task without a date is not a failure — it is a task you have
not decided when to do yet. Forcing a date at capture time forces a
decision you are not ready to make.

**Why is there no priority field?**
Priority is a function of context: time of day, energy, who's around,
what is blocked. A static field cannot capture that. Order within Today
does the job better.

**Why simple recurrence only?**
Complex recurrence rules (every second Tuesday of a month unless it
falls on a holiday, etc.) are a productivity trap. They turn a task
into a configuration problem. Daily, weekly, monthly covers most real
needs.

**Why no tagging system?**
Because a tag system with no hierarchy becomes unusable past about 15
tags, and a tag system *with* hierarchy is just projects with different
names. Flat lists are a deliberate simplification.

**Why no AI features?**
Because the value of a todo app comes from the clarity of the core
loop. AI cannot fix a confusing product, and it can make a clear one
noisy. The core loop comes first, always.

---

## Status

Larder is an actively developed personal project. The core loop
(capture → triage → do → complete) is the foundation; everything else
is built on top of it and can be cut without breaking it.

Currently working:

- Auth and per-user isolation
- Capture and Inbox
- Today with manual order
- Upcoming
- Flat lists
- Complete with undo
- Search and archive
- Export and account deletion

In progress or planned:

- Due dates and reminders
- Simple recurrence
- Accessibility pass
- Mobile layout polish

Anything not on the list above is not being worked on. The exclusion
list is a real exclusion list.

---

## Built with

- Laravel 12 (PHP 8.2+)
- Livewire 3
- Blade + Laravel Breeze
- SQLite for local development, PostgreSQL in production

The stack was chosen for one reason: it lets a small team (or one
person) ship a server-rendered, mostly-JavaScript-free app with
authentication, validation, policies, queues, and scheduling already
solved. Every one of those things would otherwise be a project of its
own.

---

## Running it locally

```bash
git clone <repo> larder
cd larder

composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
npm install
npm run dev        # in one terminal
php artisan serve  # in another