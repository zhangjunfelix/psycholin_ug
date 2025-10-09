+++
title = "Chapter 4 🧩 Sentence Processing I"
date = "2025-05-24T10:03:44-04:00"
draft = false
weight = 8
+++



# Chapter 4 Lecture Notes: Sentence Processing  
*Key Focus: Structural Ambiguity, Parsing Models, & Constraint-Based Processing*  



## Overview
This chapter examines how we convert linear word sequences into hierarchical sentence structures, focusing on how we resolve structural ambiguities in real time. We compare competing models of sentence parsing - from syntax-first garden path theory to interactive constraint-based approaches - and explore how multiple cues (syntax, semantics, context, frequency) guide our interpretation of sentences. The chapter explains why certain sentences lead to processing difficulties and how we recover from misinterpretations.


---

## Learning Goals
After studying this chapter, you should be able to:

- **Explain** structural ambiguity and how phrase structure trees represent different interpretations
- **Analyze** garden path sentences and why they cause processing difficulties
- **Compare** two-stage (garden path) and constraint-based models of sentence parsing
- **Apply** parsing heuristics (late closure, minimal attachment) to analyze sentence processing
- **Evaluate** the evidence for different constraints in sentence comprehension (context, verb frequency, animacy, prosody)
- **Understand** how visual context and referential needs influence parsing decisions
- **Explain** the tuning hypothesis and its cross-linguistic implications
- **Describe** predictive processing in sentence comprehension
- **Apply** sentence processing principles to explain real-world comprehension phenomena

---


## 1. Introduction to Sentence Processing  
### 1.1 Core Goal  
Convert linear words into hierarchical, meaningful structures to recover the speaker’s message. It relies on two fields:  
- **Syntax**: Rules/cues for word relationships (word order, prepositions).  
- **Syntactic Parsing**: How we use these cues in real time to build mental structures.  

### 1.2 Structural Ambiguity: Why Organization Matters  
Many word sequences can be grouped into phrases in multiple ways (ambiguity), leading to different meanings.  

#### Foundational Example: "Dr. Phil discussed sex with Rush Limbaugh"  
| Interpretation | Phrase Grouping | Contextual Fit |  
|----------------|-----------------|----------------|  
| 1. Discussion between two people | `[Dr. Phil] [discussed sex] [with Rush Limbaugh]` | Talk show context (they discussed sex together). |  
| 2. Sexual activity (slanderous) | `[Dr. Phil] [discussed] [sex with Rush Limbaugh]` | Sexual relationship context (he had sex with Rush Limbaugh). |  

- **Phrase Structure Trees**: Visualize hierarchy—Interpretation 1 attaches "with Rush Limbaugh" to the verb phrase (VP); Interpretation 2 attaches it to the noun phrase (NP).  

### 1.3 Key Evidence: Incremental Processing & Garden Path Sentences  
- **Immediacy Principle**: We interpret words *as soon as we see/hear them*—no waiting for the sentence end.  
- **Garden Path Sentences**: Ambiguous sentences where initial structure choices are later wrong (need revision).  

#### Classic Example: "While Susan was dressing the baby played on the floor"  
1. **Initial Ambiguity**: "dressing the baby" is parsed as "Susan dressed the baby" (attach "the baby" as object of "dressing").  
2. **Disambiguation**: "played" needs a subject—but "the baby" is already an object.  
3. **Reanalysis Cost**: Reading time at "played" is 200-300 ms slower than the unambiguous control ("While Susan was dressing herself...")—extra effort to undo the initial parse.  


## 2. Two-Stage Parsing Models (Garden Path Theory)  
Lyn Frazier’s model (1979, 1987) proposes **sequential stages**: syntax first, then semantics/context.  

### 2.1 Stage 1: Structural Analysis (Syntax-Only)  
- **Input**: Only word categories (noun, verb, preposition)—no semantics/context.  
- **Process**: Use fast, context-free heuristics to build *one* structure (prioritize simplicity).  
- **Output**: Single phrase structure tree with word roles (subject, object).  

### 2.2 Stage 2: Semantic Interpretation & Revision  
- **Input**: Stage 1 structure + word meanings + context + world knowledge.  
- **Process**: Assign thematic roles (agent, patient) and check coherence. If conflicting (e.g., garden path), revise the Stage 1 structure.  

### 2.3 Core Heuristics (Stage 1)  
Heuristics minimize processing effort and are assumed universal:  

| Heuristic | Rule | Example |  
|-----------|------|---------|  
| **Late Closure** | Attach new words to the ongoing phrase (avoid new structure). | "While Susan was dressing the baby..." → attach "the baby" to the subordinate clause (leads to garden path at "played"). |  
| **Minimal Attachment** | Build the simplest structure (fewest nodes). | "The burglar blew up the safe with the dynamite" → attach "with the dynamite" to VP ("blew up") (simpler) vs. NP ("safe"). |  
| **Main Assertion Preference** | Attach new info to the main clause (core message). | "The woman delivered the bread that she baked to the store" → attach "to the store" to main clause ("delivered") vs. subordinate clause ("baked"). |  

### 2.4 Limitations  
1. Ignores early context/semantics: Can’t explain why story context resolves ambiguity before disambiguating words.  
2. Fails cross-linguistic differences: Heuristics (e.g., late closure) aren’t universal—preferences depend on language frequency.  


## 3. Constraint-Based Parsing Models  
One-stage, parallel models (MacDonald et al., 1994; Tanenhaus et al., 1995) where all cues (syntax, semantics, context) interact simultaneously.  

### 3.1 Core Principles  
1. **Parallel Activation**: Multiple structures are activated at once (not just one).  
2. **Constraint Satisfaction**: Structures compete—more cue support = higher activation.  
3. **No Syntax Bias**: All cues influence activation from the start.  

### 3.2 Key Constraints (Cues) & Evidence  
Cues are tuned to past experience (tuning hypothesis):  

| Constraint | Description | Example/Experiment |  
|------------|-------------|--------------------|  
| **Story Context** | Referential needs (e.g., distinguishing two objects) prioritize structures. | Precede "The burglar blew up the safe with the rusty lock" with a story about two safes → fast reading (no revision needed). |  
| **Verb Subcategory Frequency** | Verbs have stable structure preferences (e.g., "realized" often takes sentence complements). | "The student realized the answer was..." → fast reading (matches preference); "The student saw the answer was..." → slow (violates preference). |  
| **Cross-Linguistic Frequency** | Preferences match language corpus frequency. | Spanish: Relative clauses attach to first nouns ("la criada de la actriz que..."); English: Attach to second nouns. |  
| **Semantic (Animacy)** | Animate nouns = likely agents; inanimate = likely patients. | "The evidence examined by the lawyer..." → fast (inanimate "evidence" can’t be agent); "The defendant examined by the lawyer..." → slow (animate "defendant" is initially parsed as agent). |  
| **Prosody** | Pauses/pitch signal phrase boundaries. | "Susie learned that Bill [pause] telephoned after John visited" → "after John visited" modifies "telephoned" (prosody guides parsing). |  
| **Visual Context** | Scene objects resolve ambiguity fastest. | "The girl placed the apple on the towel in the box":<br>- 1 apple → look at empty towel (goal);<br>- 2 apples (one on towel) → look at towel apple (modifier). |  

### 3.3 Tuning Hypothesis  
Parser weights cues based on past experience (e.g., "animate nouns = agents 80% of the time" → weight animacy heavily).  


## 4. Interim Summary: Model Comparison  
| Aspect | Two-Stage (Garden Path) | Constraint-Based |  
|--------|--------------------------|------------------|  
| Stages | Two (syntax → semantics) | One (all cues interact) |  
| Structure Activation | Serial (one at a time) | Parallel (multiple activated) |  
| Cues Used | Only word categories (Stage 1) | All (context, frequency, semantics, etc.) |  
| Garden Path Cause | Heuristic errors | Temporary competition between structures |  
| Cross-Linguistic Fit | Universal heuristics | Language-specific frequency tuning |  

### 4.1 Predictive Processing (Extension)  
Parser actively predicts upcoming words/structures (not just reacts):  
- Example: "The boy will eat..." → participants look at cake (food) *before* hearing "cake" (uses verb semantics to predict).  
- Predicts at multiple levels: phonological (sound), syntactic (category), semantic (meaning).  


## Quick Review Questions  
1. What is structural ambiguity? Give an example.  
2. Why do garden path sentences cause slowdowns?  
3. What is the key difference between two-stage and constraint-based models?  
4. Name two constraints that guide constraint-based parsing.  
5. How does the tuning hypothesis explain cross-linguistic parsing differences?