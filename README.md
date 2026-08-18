# Zero to AI Systems Engineer — Foundations (Free)

Welcome. This free course takes you from **never having written a line of code** to a working
machine learning model that other programs can call over the internet, packed in a container
that runs anywhere.

Six chapters. No experience needed. We start at *truly* zero.

> Every chapter folder holds a gentle, tiny-step guide **and the runnable scripts** for that
> chapter, so you can read it, run it, and learn at your own pace.

## What you'll have built by the end

A fraud-detection system that:

1. Learns from example transactions (Chapters 02–03)
2. Keeps a tidy record of every experiment you run (Chapter 04)
3. Answers requests from other programs over the web (Chapter 05)
4. Runs identically on any computer, packed in a container (Chapter 06)

That is a real machine learning system — the same shape the pros ship.

## How this course teaches

- **Tiny steps.** Every chapter is broken into small steps. You always know the *one* thing
  to do next.
- **Plain words first.** We explain the idea with an everyday picture (a lunchbox, a robot
  builder, a pen pal) *before* showing any code.
- **Try-it-yourself.** Each chapter ends with little challenges so you *do*, not just read.
- **"If it breaks" help.** Beginners hit errors. We list the common ones and how to fix them.
- **Free to run.** Everything here runs on your own laptop. No cloud account, no credit card,
  no surprise bills.

## The labels you'll see at the top of each chapter

| Label | What it means |
|---|---|
| 💻 **Runs free on your laptop** | You can fully do this with just your computer. No account, no money. |
| 🌐 **Needs the internet** | The chapter talks to something online. |
| 🧑‍🤝‍🧑 **Easier with a helper the first time** | Setup is fiddly; a more experienced person nearby helps a lot. |

## The six chapters

1. [Chapter 01 — Set up your computer and say hello](chapter-01-setup) · 💻
   Install Python, VS Code, and Git. Write and run your first program.
2. [Chapter 02 — Your very first tiny AI experiment](chapter-02-data) · 💻
   Make the computer learn from examples and spot fake purchases.
3. [Chapter 03 — Teach the computer to spot trouble](chapter-03-models) · 💻
   A real fraud detector with a report card, plus an anomaly finder for hospital readings.
4. [Chapter 04 — Keep a tidy notebook of your experiments](chapter-04-mlflow) · 💻
   Track every run with MLflow so you never lose your best model again.
5. [Chapter 05 — Let other programs talk to your model](chapter-05-api) · 💻 🌐
   Wrap your model in an API other software can call.
6. [Chapter 06 — Pack your program into a box (Docker)](chapter-06-docker) · 💻 🧑‍🤝‍🧑
   Containerize the API so it runs the same everywhere.

## What you need before Chapter 01

Almost nothing. Just:

- A computer (Windows, Mac, or Linux).
- About 30 minutes for the first setup.
- Curiosity. That's it.

Chapter 01 installs everything else, slowly, one piece at a time.

## Setting up (one time)

Chapter 01 walks you through this in detail. If you already know your way around Python:

```bash
git clone https://github.com/Here2ServeU/zero-2-ai-foundations.git
cd zero-2-ai-foundations
python3 -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Each chapter also lists the exact packages it needs, so you can install only what that chapter
uses if you prefer.

## One golden rule for beginners

> **Read the whole step, then do it. If something looks scary, it's just a new word — every
> new word is explained in the [GLOSSARY](GLOSSARY.md).**

Open the [GLOSSARY](GLOSSARY.md) in a second tab. Whenever you meet a bold word you don't
know, look it up there.

## Where this course goes next

These six chapters are the foundation. The full **Zero to AI Systems Engineer** course picks up
right where Chapter 06 ends and takes the same system all the way to production across 18
chapters — Terraform, cloud, CI/CD, Kubernetes, monitoring, self-healing AIOps, drift
detection and retraining, safe deployments, Grafana dashboards, and modern LLM work (RAG and
production LLM serving) — finishing with two full graduation systems: **NexaGuard** (bank
fraud) and **ClarityAI** (healthcare).

See [WHATS-NEXT.md](WHATS-NEXT.md) for the full outline.

---

➡ Start now: [Chapter 01 — Set up your computer and say hello](chapter-01-setup)
