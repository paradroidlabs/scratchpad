# Paradroid Labs: Reasoning Metadata & Alignment Engine (v2026.05)

This repository is not just a collection of AI prompts. It is an **operating system for human-AI cognitive alignment**.

The Paradroid framework utilizes a rigid *Bifurcated Protocol* (Thinking Block + Structured Scratchpad) to force Large Language Models to articulate their latent assumptions, map their reasoning pathways, and expose their cognitive biases *before* they generate a final output.

The result is that every chat session becomes a high-fidelity dataset of **Reasoning Metadata** and **User Alignment Delta**.

## The Paradigm Shift: The "Calibration Exhaust" Loop
Standard chat exports are functionally dead text—they show the input and the final output, losing the intermediate latent space.

By using the Paradroid OS, the chat export becomes a serialized, auditable log of *human-AI cognitive friction and resolution*. The model states its assumptions, the user corrects them, and the intent evolves.
This data can be extracted (via the `/telemetry/` schema) to create:
1.  **Hyper-Personalized Contexts:** Perfecting a system prompt tailored exactly to an individual user's friction points.
2.  **Premium Synthetic Training Data:** Generating Chain-of-Thought (CoT) data where the reasoning branches have been explicitly validated or corrected by a human in real-time.
3.  **Enterprise Metacognition:** Converting troubleshooting sessions into interactive Standard Operating Procedures.

## Repository Architecture

The repository is structured functionally into the OS, its augmentations, the underlying theory, and the telemetry tools.

### ⚙️ `/skills/core/`
The core operating system.
*   `paradroid-os.md` - The foundational protocol. Load this into your system prompt or custom instructions. It governs the invariant rules of the Bifurcated Protocol.

### 🔍 `/skills/lenses/` (Formerly Purpose-Built)
Cognitive Lenses (or Topologies) that warp the core OS to focus on specific spectrums (e.g., narrative, systemic logic, academic rigor). These act as plugins to the core protocol.
*   `gabg-app-design.md` - Game/App Build Guide Generator.
*   `deeper-research.md` - Systematic research and cross-domain synthesis.
*   `saganpad.md` - The flagship Carl Sagan persona framework.
*   *...and more.*

### 📊 `/telemetry/`
The extraction schemas and documentation for parsing chat exports to calculate the User Alignment Delta and extract actionable reasoning metadata.

### 📚 `/docs/`
The foundational theory governing the repository.
*   `/docs/pillars/` - Deep dives into the 5 Mission Pillars:
    1.  [Format is Function](docs/pillars/1-format-is-function.md)
    2.  [Calibration over Command](docs/pillars/2-calibration-over-command.md)
    3.  [Augmentation over Automation](docs/pillars/3-augmentation-over-automation.md)
    4.  [Thought-Mentorship](docs/pillars/4-thought-mentorship.md)
    5.  [Transparency as Sovereignty](docs/pillars/5-transparency-as-sovereignty.md)

### 🗄️ `/_archive-2025/`
Historical frameworks, early JSON structures, and standard prompt templates preserved for research and forking purposes.

## Quick Start

1.  **Load the OS:** Copy the contents of `/skills/core/paradroid-os.md` into your AI's system prompt or custom instructions.
2.  **Engage:** Begin your prompt. The AI will respond using the `thinking` -> `scratchpad` -> `output` format.
3.  **Calibrate:** Read the scratchpad. Identify where the model's `[TheoryOfMind]` or `[ConstraintCheck]` misalignment with your actual intent. Correct it in your next prompt.
4.  **Extract:** Export the chat log and use the `/telemetry/` schema to extract the value of that session.

---
*Free for any purpose with attribution. Fork, modify, commercialize, and distribute while maintaining the open-source spirit that drives innovation in AI reasoning frameworks.*
