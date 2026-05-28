# Pillar 2: Calibration over Command

## Concept
The traditional "prompt engineering" paradigm relies on one-shot commands: give the perfect instruction, get the perfect output. Paradroid rejects this in favor of an ongoing alignment loop.

## The Moving Target of Intent
User intent is rarely static. What a user thinks they want in prompt 1 is often refined or completely changed by prompt 4, specifically *because* they saw the model's assumptions in the scratchpad.

Therefore, the interaction is not a series of commands, but a continuous calibration. The scratchpad acts as a dial, surfacing the model's current understanding of the user's intent (`[TheoryOfMind]`), allowing the user to turn the dial (correct the assumption) in the next turn.
