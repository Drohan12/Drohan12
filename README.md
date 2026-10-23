# Rohan Doddi

**Software engineer focused on quality, correctness and applied machine learning.**
I build systems that check other systems: independent oracles, automated test infrastructure, and
the evaluation discipline that keeps machine-learning products honest. I also build the products
themselves, from computer-vision pipelines to audio tools.

Most of my work lives in private repositories. Walkthroughs, code access and demos are available on
request.

---

## Selected projects

### ScanDex: computer vision and machine learning for trading cards
*Co-founder. Private repository.*

A platform that grades trading-card condition from a photograph and prices the card against live
market comparables. It ships as a Next.js web app, a Manifest V3 Chrome extension and an Expo iOS
app, backed by Python services and a versioned grading contract.

- Detection and rectification with YOLO, RF-DETR and segmentation models, homography to a canonical
  frame, and a corner-consensus check against an independent localizer.
- Geometric centering measurement (multi-cue border fitting, SIFT and RANSAC print registration),
  and two deliberately different graders: gradient-boosted trees and a transparent rule-based
  scorer.
- A mixed-integer-programming service for batch seller decisions, and a forecasting service.
- Evaluation done properly: out-of-fold, set-grouped cross-validation, baselines, a shared
  training and serving feature function, and written-up negative results.

*Stack:* Python, FastAPI, PyTorch, XGBoost, OpenCV, TypeScript, Next.js, React, Expo, Supabase,
Turborepo.

### slot-oracle: an independent test oracle for scheduling systems
*Private repository, CI-tested.*

Computes exactly which meeting times are legal under a set of constraints, so a scheduler can be
judged against ground truth instead of its own account of itself. Two independent implementations
(interval algebra and brute-force enumeration) are cross-validated, a self-contained timezone layer
handles daylight-saving folds and gaps, and the judge itself is mutation-tested against a toy
scheduler with injected translation faults.

*Stack:* Python (standard library only), GitHub Actions.

### LOOM: a groove and chord workstation for FL Studio
*Private repository. Native VST3 on the roadmap.*

A client-side music-production tool built on the Web Audio and Web MIDI APIs. It generates chord,
bass, hook and drum parts from a song model and delivers them to FL Studio as MIDI files or a live
MIDI stream. Includes 72 custom-made samples and a set of hardware and interface design
explorations.

*Stack:* JavaScript, Web Audio, Web MIDI, Canvas, JUCE (planned).

---

## Experience

**QA automation contractor, AI scheduling startup** (2026)
Built live automated test suites across email, chat and text-message surfaces, an independent
oracle for scheduling correctness, and contributed CI jobs that authenticate without stored
credentials.
Filed and triaged reproducible defects with root-cause analysis and proposed fixes.

---

## What I care about

- Independent verification: the thing that judges a system should not share its blind spots.
- Measuring against baselines, and reporting what a model actually knows.
- Tooling that other engineers choose to use.

## Skills

Python · TypeScript · JavaScript · Test automation · CI/CD · Computer vision · Machine learning
evaluation · Web Audio / Web MIDI · FastAPI · Next.js · SQL
