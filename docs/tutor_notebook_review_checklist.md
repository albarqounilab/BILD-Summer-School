# Tutor Notebook Review Checklist

**Purpose:**  
Ensure the hands-on notebooks are clear, robust, reproducible, and pedagogically effective before Day 1. Review your assigned notebook(s) as if you were a student, and annotate or edit directly (e.g., Markdown cells, callouts) where helpful.

### Content & Pedagogy
- Walk through linearly as if seeing it for the first time.
- Set expectations per section/cell.  
  *Example:* “In the next cell we import `numpy`—we’ll need it to perform matrix arithmetic for feature normalization.”
- Clarify local goals (e.g., “Train a binary classifier on the synthetic dataset”).
- Highlight tunable parameters (learning rate, epochs, thresholds, etc.) and suggest exploratory prompts.  
  *Example:* “Try increasing the learning rate to 0.1 and observe the training loss behavior.”
- Ensure smooth narrative transitions.  
  *Example:* “Now that the model is trained with reasonable validation accuracy, we move to evaluation. Apply the saved weights to the test set and compute the confusion matrix.”

### Reproducibility & Robustness
- Verify all imports work in a fresh environment; flag hidden or undocumented dependencies.
- Ensure dependencies on prior notebooks are explicit, and provide a fallback (e.g., load a pre-trained model if training fails).
- Control or explain randomness (seeds) to make results approximately reproducible.
- Run the notebook end-to-end:  
  - No uncaught exceptions or misleading errors.  
  - Outputs are sensible and meaningful (not random or degenerate).

### Performance & Timing
- Estimate runtime for major blocks; annotate expected durations.
- Flag heavy steps and recommend mitigations (smaller data, quick mode, precomputed artifacts).
- Confirm checkpointing exists for long computations to avoid lost progress.

### Low-Resource / Failure Modes
- Test in constrained settings (limited RAM/CPU); note steps that break or become impractical.
- Make implicit assumptions explicit (e.g., GPU availability) and offer alternatives or warnings.

### Clarity of Outputs & Interpretation
- Label plots/tables clearly (titles, axes, legends, units).
- Add guiding reflection prompts.  
  *Example:* “Why did precision drop when lowering the decision threshold?”
- Include small sanity checks (e.g., class balance display).

### Documentation & Environment
- Explain non-obvious code; expand cryptic one-liners if necessary.
- Provide a “How to run” header: Python version, install instructions, expected data paths, Colab vs local notes.
- Call out exact version requirements when critical (e.g., `torch==2.0.1`).

### Usability / Student Experience
- Suppress or clean noisy/raw dumps and verbose logs unless educational.
- End with a “next steps” summary and optional extension ideas.

### Feedback & Issue Reporting
- Log issues in a shared tracker with:
  - Error reproduction steps  
  - Clarity/structure suggestions  
  - Parameter exploration ideas
- Flag readiness status:  
  - Ready as-is  
  - Minor edits needed (specify)  
  - Major revision needed (summarize)

### Optional Extras for Students
- Cheat sheet of common commands used in the notebook.
- “If things go wrong” debugging tips.
- Short curated links for background concepts (with context, not full lectures).


