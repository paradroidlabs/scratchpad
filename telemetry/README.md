# Telemetry & Alignment Protocol

*This directory replaces the concept of traditional "evals."*

In the Paradroid 2026 framework, the objective is not to run static unit tests against model outputs. The objective is to extract **Reasoning Metadata** and quantify the **User Alignment Delta** directly from active chat exports.

Because the Bifurcated Protocol forces the model to articulate its assumptions (`[TheoryOfMind]`, `[ReasoningPathway]`, `[AdversarialStress]`) before writing output, and the user subsequently corrects or validates those assumptions in their next prompt, the chat export becomes a high-fidelity dataset of *human-AI cognitive friction and resolution*.

## The Extraction Schema

To derive value from these logs, use a Telemetry Extraction Prompt (or programmatic parser) on your full chat export.

### Telemetry Meta-Prompt (v2026.05)
*Run this prompt against a finished session export to extract the Alignment Delta.*

```text
Please analyze the attached chat export, which follows the Paradroid 2026 Bifurcated Protocol.
Extract and compile the "Calibration Exhaust" data into the following JSON schema:

{
  "session_metadata": {
    "total_turns": 0,
    "primary_lenses_active": [],
    "identified_persona_mode": ""
  },
  "alignment_delta": {
    "friction_points": [
      {
        "turn_number": 0,
        "model_assumption": "[Extract from TheoryOfMind or ConstraintCheck]",
        "user_correction": "[Extract from user's subsequent prompt]",
        "resolution_status": "Aligned | Persistent Misalignment"
      }
    ],
    "total_calibration_turns": 0
  },
  "hyper_personalization_vector": {
    "inferred_user_preferences": [
      "List explicitly stated or inferred preferences (e.g., 'User prefers adversarial pushback on technical claims')"
    ],
    "recommended_context_integration": "A paragraph to be fed into the [ContextIntegration] block for future sessions with this user."
  }
}
```

## Success Scenario: The Calibration Exhaust Loop

1.  **Hyper-Personalization:** Aggregating `recommended_context_integration` across 50 sessions creates a flawless, data-backed system prompt for an individual user.
2.  **Synthetic Training Data:** These parsed logs represent premium Chain-of-Thought (CoT) data where reasoning branches have been explicitly validated or corrected by a human in real-time. It trains models *how to calibrate*, not just what to answer.
3.  **Enterprise Metacognition:** Experts using the framework naturally document their implicit knowledge as they correct the model's scratchpad. The export becomes an interactive Standard Operating Procedure.
