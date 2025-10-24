+++
title = "Chapter 3 Word Representation & Lexical Semantics"
date = "2025-05-15T10:03:44-04:00"
draft = false
weight = 6
+++

## 📖 Required Reading



## 📖 Required Reading
- **Chapter 3** from *Introduction to Psycholinguistics: Understanding Language Science* (2nd ed.) by Matthew Traxler.    
[Link to Chapter 3](/psycholinguistics/pdfs/C3.pdf)  



# Chapter 3: Word Processing (Part I)

## Overview
This chapter examines how the brain stores and processes word forms and meanings. We explore the hierarchical decomposition of words into smaller units (phonetic features → morphemes) and investigate competing theories of lexical semantics, from traditional feature-based approaches to modern embodied simulation models. The chapter explains real-world phenomena like why rare words are harder to process and how context resolves word ambiguity.


---


## Learning Goals
After studying this chapter, you should be able to:

- **Describe** the hierarchical structure of word forms (phonetic features → phonemes → syllables → morphemes)
- **Differentiate** between free vs. bound morphemes and inflectional vs. derivational morphemes
- **Explain** the evidence for morpheme-based processing (root frequency effect, pseudo-affix effect)
- **Distinguish** between sense and reference in lexical semantics
- **Evaluate** the core features approach to meaning and its limitations
- **Analyze** how semantic networks use spreading activation to represent meaning relationships
- **Compare** associationist models (HAL, LSA) and their symbol-grounding problem
- **Understand** the embodied semantics approach and its evidence from perceptual/motor systems
- **Apply** semantic processing principles to explain real-world language phenomena

---


# Chapter 3 Lecture Notes: Word Processing (Part I)  
*Key Focus: Word Form Representation & Lexical Semantics*  


## Overview  
This chapter explores how the brain stores and processes two core aspects of words: **form** (sound/spelling) and **meaning** (semantics). It begins with the "invisible work" of word processing (e.g., distinguishing "coffee" from "coffin") and breaks down:  
1. How words are mentally decomposed into hierarchical units (phonetic features → morphemes).  
2. How word meanings are represented (debating "dictionary-like features" vs. networks/embodied simulation).  
Real-world relevance: Explains why rare words (e.g., "philatelist") are harder to process than common ones, and how context clarifies ambiguous words (e.g., "bank").  


## 1. Mental Representation of Word Form  
### 1.1 Core Premise  
Words are not stored as single chunks—they are decomposed into smaller, nested units (like molecules → atoms). This reflects how the brain *actually processes* words during reading/speech.  

### 1.2 Hierarchy of Word Form Components  
| Level               | Description                                  | Examples                                                                 |
|---------------------|----------------------------------------------|--------------------------------------------------------------------------|
| **Phonetic Features** | Basic articulatory properties (how sounds are made). | /p/ = +labial (lips), -voiced (no vocal fold vibration); /b/ = +labial, +voiced (distinguishes *pat*/*bat*). |
| **Phonemes**        | Smallest sound units that change meaning.    | *cat* = /k/+/æ/+/t/; replacing /k/ with /b/ → *bat* (new meaning).       |
| **Syllables**       | Speech units (jaw open/close cycles).         | *cat* = CVC (/kæt/); *spam* = onset (/spa/) + rime (/am/).              |
| **Morphemes**       | Smallest meaningful units.                   | *cats* = *cat* (root) + *-s* (plural); *unhappy* = *un-* (negative) + *happy* (root). |

### 1.3 Morpheme Types  
| Category               | Definition                                  | Examples                                                                 |
|-------------------------|----------------------------------------------|--------------------------------------------------------------------------|
| **Free vs. Bound**      | Free = stands alone; Bound = needs a root.   | Free: *dog*, *run*; Bound: *-s* (plural), *un-* (negative).             |
| **Inflectional vs. Derivational** | Inflectional = modifies meaning (tense/number) but not part of speech; Derivational = changes part of speech. | Inflectional: *bake* → *baked* (verb → verb); Derivational: *confuse* (verb) → *confusion* (noun). |

### 1.4 Evidence for Morpheme-Based Processing  
| Effect                | Description                                                                 | Example                                                                 |
|-----------------------|-----------------------------------------------------------------------------|--------------------------------------------------------------------------|
| **Root Frequency**    | Rare full words (low surface frequency) are fast to process if their root is common (high root frequency). | *Dogpile* (rare) is processed as fast as *dog* (common) → brain uses the root *dog* to shortcut recognition. |
| **Pseudo-Affix**      | Words with fake affixes take longer to process (brain strips the affix, fails to find a root, then re-searches). | *Sister* (fake *-er*) is slower than *grower* (real *-er* = "someone who grows"). |


## 2. Lexical Semantics: What Is "Meaning"?  
### 2.1 Key Distinction: Sense vs. Reference (Jackendoff, 1983)  
| Type       | Definition                                  | Example                                                                 |
|------------|----------------------------------------------|--------------------------------------------------------------------------|
| **Sense**  | General, stable knowledge (dictionary-like). | *Cat* = "small furry mammal, purrs, hunts mice."                        |
| **Reference** | Context-specific "target" (what the word points to). | *My cat* = your specific pet (e.g., Mittens, a tabby).                  |

### 2.2 Traditional Theory: Core Features Approach  
- **Claim**: Meaning = list of "necessary features" (e.g., *bachelor* = human + adult + male + unmarried).  
- **Critiques**:  
  1. Exceptions: Monks meet "bachelor" features but are not called bachelors.  
  2. Fuzzy categories: *Game* (board/sports/video) has no universal uniting feature.  
  3. Prototypicality: "Fire engine red" is a "better" *red* than "red hair"—features treat all examples equally.  

### 2.3 Modern Theory 1: Semantic Network (Collins & Loftus, 1975)  
- **Claim**: Meaning = activation pattern in a network of nodes (concepts) and links (relationships).  
- **Components**:  
  - Nodes = concepts (*goose*, *bird*); Links = "Is a" (*goose*→*bird*), "Has" (*bird*→*feathers*).  
  - **Spreading Activation**: Activating one node (e.g., *goose*) spreads to connected nodes (*duck*, *waterfowl*)—automatic, weakens with distance.  
- **Evidence: Semantic Priming**: Faster response to *duck* if preceded by *goose* (related) than *horse* (unrelated).  

### 2.4 Modern Theory 2: Associationist Models (HAL & LSA)  
| Model       | Corpus                                  | Method                                  | Meaning Representation                          | Limitation (Symbol-Grounding Problem) |
|-------------|-----------------------------------------|-----------------------------------------|-------------------------------------------------|---------------------------------------|
| **HAL**     | 200M USENET words                      | Tracks word co-occurrence (proximity scores). | Word = vector in a 70k×70k matrix.             | No real-world grounding—only word-word links (like a Chinese Room: follows rules but doesn’t "understand"). |
| **LSA**     | 5M encyclopedia words                   | Reduces "word×episode" matrix to 300 dimensions. | Word = vector across 300 dimensions.            | Same as HAL—no connection to real objects/actions. |

### 2.5 Modern Theory 3: Embodied Semantics (Indexical Hypothesis)  
- **Claim**: Meaning is tied to perceptual/motor systems (simulate real-world experiences).  
- **3 Steps**:  
  1. **Indexing**: *Chair* → mental image of a chair (seat/back).  
  2. **Affordances**: Infer actions (chair → "can sit").  
  3. **Meshing**: Phrase meaning = combining affordances ("sit on chair" = chair’s "affords sitting" + body’s "can sit").  
- **Evidence**: Participants judge "fill sweater with leaves" (plausible, leaves afford being a pillow) as better than "fill with water" (implausible)—LSA can’t predict this.  


## Quick Review Questions  
1. What is a morpheme? Give an example of a bound derivational morpheme.  
2. How does the root frequency effect support morpheme-based processing?  
3. What’s the difference between "sense" and "reference" for the word *dog*?  
4. Why does the core features approach fail to explain word meaning?  
5. What is spreading activation in the semantic network model?