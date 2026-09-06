# Forward Deploy Starter — Lim's Learning Hub

The project folder for Forward Deploy Academy's online edition. It holds Mdm Lim's
tuition-centre data and the instructions your AI building partner reads before it
does anything. You build the application; the AI writes the code; your `spec.md`
drives it.

## What you need

- Node.js 20 or newer (`node --version`)
- git
- One AI coding tool on your machine:
  - Claude Code: `npm install -g @anthropic-ai/claude-code`
  - or Codex: `npm install -g @openai/codex`

## Set up

```sh
git clone https://github.com/haskytech-basic/forward-deploy-starter.git limshub
cd limshub
npm install
```

## Work

1. Open a terminal in this folder and start your AI tool: `claude` (or `codex`).
2. Say what Mdm Lim's problem is in your own words. Ask it to run the
   design-build-loop with you. The result is `spec.md` in this folder.
3. When the spec is done, ask it to plan the build against `spec.md`, then build.
4. Start the app it wrote: `npm start`, then open <http://localhost:3000>.
5. Check every Given / When / Then in your spec against the running app.

Your teacher on WhatsApp reviews the spec, the running app and your evidence.
The course tells you when to send what.

## What is here

| Path | What it is |
|------|------------|
| `CLAUDE.md` | The instructions the AI reads: the scenario, the design-build-loop, the stack |
| `data/students.csv` | 25 students, classes, parent contacts |
| `data/classes.csv` | The weekly timetable |
| `data/payments.csv` | Three months of payments |
| `data/attendance.csv` | Four weeks of attendance |
| `package.json` | Express and better-sqlite3, already declared |

The data is deliberately messy: phone numbers in mixed formats, a few blanks. Real
data is like that. Loading it is part of the exercise.

## Stack

Express.js for the server, SQLite (one file, `data/app.db`) for the database,
plain HTML, CSS and JavaScript for the pages. One language, nothing to install
beyond `npm install`. The production stack the academy teaches later swaps each
layer for its bigger sibling; the process stays the same.

---

Forward Deploy Academy · Hasky Technologies · Singapore
