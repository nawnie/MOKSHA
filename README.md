# RNV1

![Status](https://img.shields.io/badge/status-investor_briefing-blue)
![Stage](https://img.shields.io/badge/stage-early_prototype-green)
![Focus](https://img.shields.io/badge/focus-local_embodied_AI-purple)
![Proof](https://img.shields.io/badge/proof-ReTrain_public_tool-orange)

RNV1 is the public investor-facing page for a local AI and embodied intelligence program.

This repository is not the implementation repo. It is not where we publish private model work, internal datasets, hardware notes, control code, or partner material. The goal here is to explain the direction clearly and point to public proof that the work is backed by real software.

The first public proof is [ReTrain](https://github.com/nawnie/ReTrain), a local-first training workbench we built to support consumer GPU fine-tuning workflows. ReTrain is software we can show. RNV1 is the larger system we are building toward.

---

## The short version

RNV1 is about moving local AI beyond a chat window.

The program combines training tools, model routing, structured memory, human steering, and eventually hardware or embodied adapters. The target is a system that can be trained, inspected, corrected, and moved into practical host environments without depending on a cloud-only stack.

The public code will stay selective. Investors and partners should see enough to know we are building, but the core implementation will not be dumped into this page.

---

## Why this exists

Most AI products still treat the model as the whole system. That leaves practical gaps:

- training workflows are hard for normal users to run,
- local model behavior is hard to measure,
- long-term memory becomes messy fast,
- tool routing is usually glued together after the fact,
- hardware and runtime limits are ignored until they break the demo,
- and embodied or assistive systems need more discipline than a chatbot loop.

RNV1 is our answer to that missing operating layer.

---

## What RNV1 is

RNV1 is an early program for building a local AI operating stack around four parts:

| Part | Role |
|---|---|
| Training | Build and adapt models with repeatable local workflows |
| Runtime | Route work across local models, tools, and expert backends |
| Memory | Keep context, sources, and user intent organized enough to inspect |
| Interface | Let a person steer, correct, and evaluate the system without digging through raw code |

The long-term direction includes embodied and assistive systems. That does not mean this repo is a robot controller, medical device, or finished commercial product. It is the public front door for the research and prototype path.

---

## Proof we are building

### ReTrain

[ReTrain](https://github.com/nawnie/ReTrain) is the clearest public artifact right now.

It is a local-first training workbench for consumer GPU fine-tuning. It includes:

- a Gradio 6 training UI,
- QLoRA as the first consumer GPU training engine,
- tune-scope controls for safer experiments,
- Hugging Face model download staging,
- VRAM safety checks before training,
- data recipe and vision dataset builders,
- TensorBoard support,
- dry-run receipts,
- and a JSON FastAPI bridge for a later React frontend.

We use ReTrain as part of the RNV1 build path because RNV1 needs training tools we can run and inspect locally. It is public so investors can see actual software instead of only a pitch.

### Model Operating Kernel

[Model Operating Kernel](https://github.com/nawnie/Model-Operating-Kernel) is the runtime side of the work. It coordinates model and expert backends, records traces, tracks VRAM pressure, and creates evaluation data for routing decisions.

### AIWF Research Atlas

[AIWF Research Atlas](https://github.com/nawnie/ai-without-fear) is the retrieval and source-discipline side. It keeps source policy, topic lanes, retrieval cards, and AI workflow material in a structure that local assistants can index.

Together, these projects show the shape of the RNV1 stack: train locally, route locally, remember with sources, and keep claims testable.

---

## What is private

RNV1 is investor-facing, not an open implementation dump.

The following stay private unless there is a clear release reason:

- internal model weights and adapters,
- unpublished datasets,
- private training runs,
- hardware integration notes,
- partner conversations,
- safety notes that should not be public,
- prototype control logic,
- and internal architecture details that create copy risk before funding.

Public repos are used as proof-of-work and context. They are not the whole system.

---

## Near-term milestones

| Milestone | Why it matters |
|---|---|
| Harden ReTrain training flows | RNV1 needs repeatable local model adaptation |
| Connect training receipts to evaluation | Claims need run records, not vibes |
| Expand MoK routing tests | Runtime decisions need measurable behavior |
| Build RNV1 memory examples | Long-term behavior needs inspectable context |
| Prepare investor demo material | Partners need a clear view without private code exposure |
| Define first host-adapter target | Embodied work needs a concrete environment, not a broad promise |

---

## Funding and partner fit

RNV1 is relevant to partners working on:

- local AI systems,
- consumer GPU training,
- assistive technology,
- robotics research,
- smart environments,
- human-machine interfaces,
- AI education and workforce tools,
- model evaluation,
- and privacy-preserving AI workflows.

The immediate funding need is not just model training. It is productizing the local stack around training, runtime control, memory, evaluation, and usable interfaces.

---

## Current status

**Public stage:** investor briefing and proof-of-work index  
**Build stage:** early prototype stack  
**Public proof:** ReTrain, Model Operating Kernel, AIWF Research Atlas  
**Code release posture:** selective public tools, private core implementation  
**Main goal:** turn local AI training, routing, memory, and interface work into a fundable RNV1 prototype

This page will change as the public RNV1 repo and investor materials are cleaned up.
