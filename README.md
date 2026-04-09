# Binding Assay Reasoning Benchmark

A benchmark for evaluating scientific reasoning in binding assay interpretation, experimental design, and failure-mode analysis.

---

## Why this benchmark exists

Most current biology benchmarks test **recall or constrained Questions and Answers**.

Real biological research is different.

Scientists must:

* Interpret noisy and ambiguous assay results
* Understand assay-specific artifacts (SPR, BLI, ELISA, etc.)
* Avoid overclaiming from limited evidence
* Design the *right next experiment*, not just explain results

This benchmark evaluates whether models can reason through **realistic binding assay scenarios**, not just retrieve facts.

---

## Why binding assays?

Binding assays are an ideal testbed for scientific reasoning because:

* Results are often **ambiguous and context-dependent**
* Assay format strongly influences outcomes
* Artifacts (nonspecific binding, avidity, surface effects) are common
* Multiple hypotheses can explain the same signal
* Correct conclusions require **careful qualification**
* Expert analysis is needed to translate binding parameters to a actual outcome for the assay

---

## 📊 Benchmark Structure

The benchmark is organized into 4 task families:

### 1. Assay Interpretation

Interpret results from assays like SPR, BLI, ELISA.

### 2. Experimental Design

Identify the best follow-up experiment.

### 3. Evidence Integration

Combine multiple pieces of assay data to reach a conclusion.

### 4. Failure Mode Analysis

Critique flawed reasoning or model outputs.

---

## 🧩 Example Benchmark Item

**Prompt:**

> An antibody shows strong binding in SPR but no measurable signal in ELISA.
> What are the most plausible explanations, and what experiment would you perform next?

**Expected reasoning includes:**

* Assay format differences (surface immobilization vs plate binding)
* Epitope accessibility issues
* Detection sensitivity differences
* Need for orthogonal validation

---

## 📏 Evaluation Criteria

Responses are scored across:

* Scientific correctness
* Use of evidence
* Recognition of ambiguity
* Assay-specific reasoning
* Quality of proposed experiments
* Calibration (avoiding overclaiming)

---

## ⚠️ Common Failure Modes

* Overclaiming from limited evidence
* Ignoring assay format differences
* Confusing affinity vs specificity
* Treating noisy data as definitive
* Missing need for orthogonal validation

---

## 📂 Repository Structure

```
data/          Benchmark dataset (JSON)
docs/          Benchmark design and principles
src/           Evaluation scripts
examples/      Model outputs and analysis
notebooks/     Exploration and evaluation
```

---

## 🔬 Scientific Rigor

* Benchmark items are **expert-authored**
* Designed to reflect **real experimental ambiguity**
* Emphasis on **reasoning quality**, not just correctness
* Supports multiple valid hypotheses when justified

---

## 🚧 Roadmap

* v1: Expert-authored benchmark (40–60 items)
* v2: Literature-derived scenarios
* v3: Expert annotation + inter-rater agreement
* v4: Multimodal inputs (sensorgrams, curves)

---

## 📜 Citation

If you use this work, please cite:

(see `CITATION.cff`)
