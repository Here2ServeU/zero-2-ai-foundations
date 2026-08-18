# What's next after Chapter 06

You finished the foundations. Take a second to notice what that means: you installed a real
development setup, trained real models, tracked real experiments, served a model over an API,
and shipped it in a container. Most people who say they "want to get into AI" never get this
far.

## What you can already do

- Write and run Python programs
- Train a supervised model and read its report card honestly (what it caught, what it missed)
- Find anomalies with no labels at all
- Track every experiment so your best model is never lost
- Serve a model behind an HTTP API
- Package the whole thing in Docker so it runs anywhere

That is the "it works on my laptop" milestone. The gap between here and a system a company
trusts with real money and real patients is everything that happens *after* the container is
built.

## The gap this course closes

| You can do now | What production also needs |
|---|---|
| Run the container on your laptop | Real infrastructure, provisioned repeatably |
| Deploy by hand | A pipeline that tests and ships for you |
| One container | Many copies, healing themselves, scaling with traffic |
| Check the output yourself | Metrics, alerts, and dashboards that watch it for you |
| A model trained once | Drift detection and automatic retraining as the world changes |
| A model that predicts | LLMs that read your own documents and answer in plain English |

## The full course — Zero to AI Systems Engineer (18 chapters)

Picks up exactly where Chapter 06 ends, same voice, same tiny-step style.

**Part 2 — Make it run anywhere**
- Chapter 07 — Rent a computer with a wish-list (Terraform)
- Chapter 08 — Build bigger in the cloud
- Chapter 09 — A robot helper that checks your work (CI/CD)
- Chapter 10 — Run many copies safely (Kubernetes)

**Part 3 — Make it watch and heal itself**
- Chapter 11 — Watch your program's health (Monitoring)
- Chapter 12 — Teach the system to fix itself (AIOps)
- Chapter 13 — Notice when the world changes (Drift & retraining)
- Chapter 14 — Release changes without scary surprises
- Chapter 15 — Dashboards you can watch (Grafana)

**Part 4 — Modern AI: smart writing robots**
- Chapter 16 — Talk to a smart writing robot (LLM)
- Chapter 17 — Give the robot your own notes to read (RAG)
- Chapter 18 — Run the smart robot for real (Production LLM)

**Graduation projects** — two complete systems you build end to end:
- **NexaGuard** — real-time bank fraud detection
- **ClarityAI** — healthcare risk and readmission, with compliance built in

## Join the full course

<!-- TODO: replace with your live enrollment link before publishing -->
➡ **[Enroll in Zero to AI Systems Engineer](https://emmanuelnaweji.com)**

Questions, or want to show what you built in these six chapters? Open an issue on this repo —
I read them.
