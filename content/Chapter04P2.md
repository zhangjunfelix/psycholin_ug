+++
title = "Chapter 4 🧩 Sentence Processing II"
date = "2025-05-27T10:03:44-04:00"
draft = false
weight = 9
+++


# Chapter 4 Lecture Notes: Sentence Processing II  
*Key Focus: Argument Structure, Parsing Model Limitations, & Long-Distance Dependencies*  


## Overview  
This chapter extends sentence processing by addressing three critical topics:  
1. **Argument Structure Hypothesis (ASH)**: Solves the "storage dilemma" of constraint-based models by distinguishing mandatory verb arguments (core partners) from optional adjuncts (extra details).  
2. **Limitations of Constraint-Based Models**: Why simplicity sometimes overrides frequency, and alternative theories (Construal, Good-Enough Parsing, Race-Based) that blend two-stage and constraint-based ideas.  
3. **Long-Distance Dependencies**: How we link separated words (e.g., *the boy* in "It was the boy whom the girl chased") via gaps/traces or direct verb linking.  


---



## Learning Goals
After studying this chapter, you should be able to:

- **Differentiate** between arguments and adjuncts and explain their distinct processing characteristics
- **Apply** the Argument Structure Hypothesis to explain verb frame limitations and processing differences
- **Analyze** the key limitations of constraint-based parsing models and the evidence supporting them
- **Compare** alternative parsing theories (Construal, Good-Enough, Race-Based) and their unique claims
- **Explain** how we process long-distance dependencies using gaps-and-traces versus direct verb linking
- **Evaluate** the evidence for active filler strategy in ambiguous gap sentences
- **Apply** sentence processing principles to explain real-world comprehension phenomena and parsing difficulties
- **Understand** how different parsing theories account for both efficient processing and comprehension errors

---


## 1. Argument Structure Hypothesis (ASH)  
### 1.1 Core Problem: The "Storage Dilemma"  
Constraint-based models struggle to explain how we store endless verb structures (e.g., *read* can be intransitive/transitive/ditransitive). ASH solves this by splitting verb partners into **arguments** (mandatory, pre-stored) and **adjuncts** (optional, computed dynamically).  

### 1.2 Arguments vs. Adjuncts: Key Differences  
| Criterion               | Arguments (Mandatory)                          | Adjuncts (Optional)                          |  
|-------------------------|------------------------------------------------|----------------------------------------------|  
| **Obligatoriness**      | Cannot omit (sentence is ungrammatical).       | Can omit (core meaning remains).              |  
| **Semantic Necessity**  | Fill a "meaning gap" in the verb (e.g., *devour* needs something to devour). | Add extra details (time/location/manner).     |  
| **Lexical Link**        | Stored with the verb in the mental lexicon.    | Not tied to the verb’s lexical entry.         |  

#### Examples  
- **Arguments**:  
  - *Devour* (transitive): *Dr. Phil devoured the sandwich* (grammatical); *Dr. Phil devoured* (ungrammatical—no object).  
  - *Put* (triadic): *Dr. Phil put the book on the shelf* (grammatical); *Dr. Phil put the book* (ungrammatical—no goal).  
- **Adjuncts**:  
  - *Quickly* in *Dr. Phil devoured quickly* (optional—sentence is complete without it).  
  - *At the park* in *Dr. Phil put the book on the shelf at the park* (optional—core action intact).  

### 1.3 Verb Argument Frames (Stored in Lexicon)  
Each verb’s lexical entry includes an **argument frame** (0–4 arguments max, cognition limits this number):  

| Verb Type               | Definition                                  | Example                                      |  
|-------------------------|----------------------------------------------|----------------------------------------------|  
| **Zero-Argument**       | No real arguments (weather verbs; *it* = dummy subject). | *It rained*; *It snowed*.                    |  
| **One-Argument (Intransitive)** | Requires only a subject (agent).           | *Dr. Phil sneezed*; *The baby cried*.        |  
| **Two-Argument (Transitive)**   | Requires subject + direct object (patient).  | *Dr. Phil devoured the sandwich*.             |  
| **Three-Argument (Ditransitive)** | Requires subject + direct object + goal/recipient. | *Dr. Phil gave Rush Limbaugh a book*; *Dr. Phil gave a book to Rush Limbaugh*. |  
| **Four-Argument (Rare)**        | Requires agent + opponent + stake + event (betting/contract verbs). | *Dr. Phil bet Rush Limbaugh a sandwich that Big Brown would win*. |  

### 1.4 Evidence for ASH  
#### 1. Faster Processing of Arguments  
Arguments are pre-stored → faster integration than adjuncts.  
- **Experiment (Clifton et al., 1991)**:  
  - (51) *The saleswoman tried to interest the man in the wallet* (argument: *in the wallet* = required by *interest*).  
  - (52) *The saleswoman interested the man in his fifties* (adjunct: *in his fifties* = describes *the man*).  
- **Result**: Reading times for (51) are 100–150 ms faster—parser retrieves argument frames, computes adjuncts on the fly.  

#### 2. Argument Interpretation Bias  
Ambiguous phrases are initially parsed as arguments (pre-stored) before revision.  
- **Example**: *The bully stapled a letter to Harry* → *to Harry* is first parsed as an argument (goal for *stapled*) → revised if semantics conflict (odd to "staple to Harry").  
- **Evidence**: Longer eye fixations at *to Harry*—reflects revision.  

#### 3. Inference of Missing Arguments  
Omitted arguments are automatically inferred (adjuncts are not).  
- **Experiment (Mauner et al., 1995)**:  
  - *The ship was sunk* (passive, needs agent) → infer "by someone".  
  - *The ship sank* (intransitive, no agent) → no inference.  
- **Result**: Purpose clauses (*...to collect insurance*) are 200 ms faster for *was sunk*—inferred agent links to the purpose.  


## 2. Limitations of Constraint-Based Models & Alternatives  
### 2.1 Key Limitations  
#### 1. Simplicity Overrides Frequency  
Constraint-based models predict frequent structures are preferred—but simplicity (minimal attachment) wins, causing garden paths.  
- **Example (Pickering et al., 2000)**: *The athlete realized her shoes somehow got left on the bus* → *realized* usually takes sentence complements (90% frequency), but parser initially parses *her shoes* as a direct object (simpler) → slowdown at *somehow*.  

#### 2. No "Reverse" Garden Paths  
Context favoring complex structures does not interfere with simple structures (contradicts constraint-based competition).  
- **Example (Binder et al., 2001)**: *The criminal exiled his partner...* → reading times are identical in 1-criminal (simple) and 2-criminal (complex) contexts—no interference.  

### 2.2 Alternative Parsing Theories  
#### 1. Construal Theory (Frazier & Clifton, 1996)  
- **Core**: Parse arguments (primary relations) sequentially (two-stage: syntax-first) and adjuncts (non-primary) in parallel (constraint-based).  
- **Example: Relative Clauses**:  
  - *The daughter of the colonel who had a black dress left* → *who...* is an adjunct (parallel processing) → semantics (dress = daughter) quickly selects correct structure → no slowdown.  

#### 2. Good-Enough Parsing (Ferreira, 2003)  
- **Core**: Comprehenders build "good-enough" (not perfect) structures—stop parsing when meaning is clear.  
- **Evidence**:  
  - *The mouse was eaten by the cheese* → most paraphrase as *The mouse ate the cheese* (ignore passive syntax, use semantics).  
  - *While the hunter stalked the deer drank...* → 70% answer "yes" to "Was the hunter stalking the deer?" (retain initial misparse—good enough for gist).  

#### 3. Race-Based Models (Van Gompel et al., 2005)  
- **Core**: Multiple structures "race" to reach activation threshold—first to win is selected; reanalysis if wrong. No weighted activation (all start equal).  
- **Example: Garden Path Sentence**:  
  - Structure 1 (*the baby* = object of *dressing*) activates faster (simpler) → wins first → slowdown at *played* (reanalysis to Structure 2: *the baby* = subject of *played*).  
- **Evidence: Structural Priming**: Prime sentences speed up activation of matching structures in the race.  


## 3. Parsing Long-Distance Dependencies  
### 3.1 Local vs. Long-Distance Dependencies  
- **Local**: Related words are adjacent (e.g., *The girl chased the boy*—subject/verb, verb/object are next to each other).  
- **Long-Distance**: Related words are separated (e.g., *It was the boy whom the girl chased*—*the boy* is separated from *chased* by *whom the girl*).  

### 3.2 Two Theories of Long-Distance Parsing  
#### 1. Gaps-and-Traces Theory (Chomsky, 1965)  
- **Core**: Moved words (*fillers*, e.g., *the boy*) leave a **gap** (placeholder) in their original position; parser links filler to gap via a "trace".  
- **Parsing Steps for *It was the boy whom the girl chased***:  
  1. Detect *the boy* as a filler (signaled by *It was... whom*).  
  2. Search for a gap (after a transitive verb needing an object).  
  3. Find gap after *chased* → link *the boy* to gap.  
- **Evidence: Cross-Modal Priming (Nicol & Swinney, 1989)**:  
  - Filler (*the boy*) is reactivated at the gap → faster naming of *boy* or *child* (associate) at the gap vs. before the verb.  

#### 2. Gap-Free Theory (Pickering & Barry, 1991)  
- **Core**: No gaps/traces—link filler directly to the verb that requires it (use verb’s argument frame).  
- **Parsing Steps for *It was the boy whom the girl chased***:  
  1. Detect *the boy* as a potential direct object.  
  2. When encountering *chased* (needs direct object), link *the boy* directly to *chased*.  
- **Evidence: Verb-Based Slowdown (Pickering & Traxler, 2001)**:  
  - (68) *That’s the pistol with which the killer shot the man* (sensible: *pistol* = instrument for *shot*).  
  - (69) *That’s the pistol in which the killer shot the man* (nonsensical: *pistol* ≠ location).  
- **Result**: Slowdown at *shot* (not gap) for (69)—parser links filler to verb when verb is encountered, not at gap.  

### 3.3 Active Filler Strategy (Ambiguous Gaps)  
For sentences with multiple possible gaps, parser attaches filler to the **first possible gap** (even if wrong).  
- **Example (Stowe, 1986)**: *That’s the boy that the girl liked [doubtful gap] to ignore [real gap]* → parser first links *the boy* to gap after *liked* → revises at *to ignore*.  
- **Evidence**: 250 ms slowdown at *to ignore* (revision effort).  


## Quick Review Questions  
1. What is the difference between an argument and an adjunct? Give an example of each.  
2. Why does ASH limit verbs to 4 arguments?  
3. What is "good-enough parsing"? Give an example of when it occurs.  
4. How do gaps-and-traces theory and gap-free theory differ in parsing long-distance dependencies?  
5. What is the active filler strategy, and when does it cause processing slowdowns?