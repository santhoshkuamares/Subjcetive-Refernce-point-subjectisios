# Subjetesis  Framework: AI Simulation

This repository contains a small proof-of-concept implementation of the Subjetesis  framework. The simulation operationalises the framework as a recursive gap-reduction process:

`Subjective Reference Point → Broad SRP-anchored gap → Candidate sub-goals → Selected sub-goal as Norm of Study → Inquiry action → Subjetesis  monitoring → Residual gap evaluation → Post-hoc observation`

## Purpose

The implementation does not claim that the language model is conscious, self-aware, or biologically equivalent to the human brain. The model is used as a semantic simulator. It generates candidate sub-goals, selects an operative Norm of Study, carries out an inquiry action, and evaluates the result using formal variables from the Subjetesis  framework.

The key design principle is separation between generation and observation. During generation, the model is not instructed to simulate reflective self-awareness, existential self-awareness, Theory of Mind, flow, meaning-making, existential dread, awe, confusion, or insight. These patterns are only assessed after the simulation output has been generated.

## Model Structure

The cognitive state is represented as:

```text
X_t = (R_t, U_t, Γ_t, S_t, N_t, A_t, M_t)
```

where:

- `R_t` = Subjective Reference Point
- `U_t` = current world-model or understanding
- `Γ_t` = broad SRP-anchored information gap
- `S_t` = candidate sub-goals
- `N_t` = selected sub-goal functioning as the operative Norm of Study
- `A_t` = possible inquiry actions
- `M_t` = Subjetesis  metacognitive monitoring process

## Priority Equation

Each candidate sub-goal is scored using:

```text
P_t(s_i) = w1Rel_t(s_i) + w2IG_t(s_i) + w3Sol_t(s_i) + w4CP_t(s_i) + w5Val_t(s_i) - w6Cost_t(s_i) - w7Risk_t(s_i)
```

The highest-priority candidate becomes the operative Norm of Study:

```text
N_t = argmax P_t(s_i)
```

## Subjetesis  Monitoring Equation

After the selected action is carried out, progress is evaluated using:

```text
I_t = η1ΔC_N + η2ΔC_Γ + η3ΔCoh_t + η4Ev_t - η5FCR_t
```

where:

- `ΔC_N` = progress in closing the selected Norm of Study
- `ΔC_Γ` = progress in reducing the broader SRP-anchored gap
- `ΔCoh_t` = increase in coherence
- `Ev_t` = evidence grounding
- `FCR_t` = false closure risk

## Files

- `Subjetesis _simulation.py`  
  Main Python script. Paste the final simulation code from the Colab notebook into this file.

- `requirements.txt`  
  Python dependencies.

- `sample_output.md`  
  Example output from the simulation. Replace the template text with your actual Colab results.

- `.gitignore`  
  Files and folders that should not be uploaded to GitHub.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git
cd YOUR-REPOSITORY-NAME
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the simulation:

```bash
python Subjetesis(1).py
```

## Suggested Colab Use

This project was developed for Google Colab. If running in Colab, install the dependencies first:

```python
!pip install -r requirements.txt
```

Then run the notebook or copy the code from `Subjetesis(1).py`.

## Disclaimer

This repository is a conceptual and computational proof-of-concept. It does not provide empirical proof of consciousness, biological selfhood, or subjective experience. It demonstrates that the Subjetesis  framework can be operationalised as a recursive gap-reduction pipeline for future theoretical, empirical, and computational work.

## Citation

If using this repository in a paper, cite it as:

```text
Elumalai ~Srinivasan, Santhosh (2026) Subjetesis  Framework: AI Simulation. GitHub repository. Available at: INSERT-GITHUB-LINK-HERE (Accessed: INSERT-DATE-HERE).
```
