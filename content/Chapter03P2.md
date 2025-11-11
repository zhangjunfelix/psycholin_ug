+++
title = "Chapter 3 Lexical Access & Lexical Ambiguity Resolution"
date = "2025-05-19T10:03:44-04:00"
draft = false
weight = 7
+++


# Chapter 3: Word Processing (Part II)  
*Key Focus: Lexical Access, Ambiguity Resolution, & Neural Bases*  


## Overview
This chapter explores how we access words from mental storage during listening and reading, examining competing models of lexical access and how we resolve ambiguous words. We investigate the neural basis of word processing, from brain regions specialized for different word types to debates about localized versus distributed semantic representation. The chapter connects computational models with neuropsychological evidence to explain real-world language processing.

---

## Learning Goals
After studying this chapter, you should be able to:

- **Define** lexical access and explain the evidence for its speed and automaticity
- **Compare** first-generation (Logogen, FOBS), second-generation (TRACE, COHORT), and third-generation (SRN, DCM) models of lexical access
- **Analyze** how different models handle word frequency effects, context, and ambiguity
- **Explain** the key findings from Swinney's ambiguity experiments and their implications
- **Differentiate** between exhaustive access and context-dependent models of ambiguity resolution
- **Identify** the major brain regions involved in auditory/visual word form processing and semantic access
- **Evaluate** neuroimaging evidence for embodied semantics and category-specific activation
- **Compare** localized versus distributed theories of semantic representation in the brain
- **Apply** lexical processing principles to explain real-world language phenomena and neuropsychological cases

---


## 1. Lexical Access  
### 1.1 Core Definition  
Lexical access = the mental processes that activate a word’s form (sound/spelling) during listening/reading. It is *fast* (e.g., "fast shadowers" repeat speech with a 250 ms lag—1 syllable behind) and integrates form + context (errors like "cat" → "dog" [semantic fit] vs. "table" [no fit]).  

### 1.2 Foundational Evidence for Speed  
| Task               | Description                                                                 | Result                                                                 |
|--------------------|-----------------------------------------------------------------------------|-----------------------------------------------------------------------|
| **Word Monitoring** | Press a key when hearing a target phoneme (e.g., /s/).                     | Faster responses for /s/ in real words ("sun") vs. non-words ("sulx"); faster for high-frequency words ("sun") vs. low-frequency ("silt"). |
| **Gating Task**    | Hear short word snippets (25 ms, 50 ms) and guess the word.                | 1-2 syllable words in sentences need ~200 ms of input for correct identification; isolated words need ~100 ms more (context accelerates access). |

### 1.3 Models of Lexical Access  
Models differ in *information flow* (bottom-up vs. interactive) and *representation* (discrete vs. distributed).  

#### A. First-Generation (Bottom-Up, Serial)  
Strictly low-level features → high-level word forms; no top-down feedback.  

##### 1. Logogen Model (Morton, 1969)  
- **Architecture**: Each word has a "logogen" (evidence-collecting unit) with an activation threshold. Input comes from:  
  1. Auditory/visual analysis (e.g., /kæt/ or "cat").  
  2. Context (semantic links raise activation).  
  3. Rehearsal (recent words have lower thresholds).  
- **Key Rules**:  
  - Threshold exceeded → word form/meaning accessed.  
  - High-frequency words (e.g., "cat") have lower thresholds (faster access).  
- **Successes**: Explains frequency effects (common words = fast) and noise resistance (high-frequency words recognized in noise).  

##### 2. FOBS Model (Taft & Forster, 1975)  
- **Architecture**: Words grouped into "root morpheme bins" (e.g., "dog" bin includes "dog," "dogs," "dogpile"); ordered by surface frequency.  
- **Process**:  
  1. Strip affixes (e.g., "dogs" → root "dog").  
  2. Search the "dog" bin (start with high-frequency entries like "dog" before "dogged").  
- **Evidence**:  
  - **Root Frequency Effect**: "Dogpile" (rare full word) is fast to process (root "dog" is common).  
  - **Pseudo-Affix Effect**: "Sister" (fake "-er") is slow—brain strips "-er," fails to find "sist," then re-searches with full word.  

#### B. Second-Generation (Interactive, Parallel)  
Top-down feedback + parallel activation of multiple candidates.  

##### 1. TRACE Model (McClelland & Elman, 1986)  
- **Architecture**: 3-layer network (feature → letter/phoneme → word) with:  
  - **Cascaded Activation**: Units send input immediately (no waiting for full activation).  
  - **Lateral Inhibition**: Same-layer units suppress each other (e.g., "A" inhibits "T" to resolve ambiguity).  
  - **Top-Down Feedback**: Word units boost component letters/phonemes (e.g., "WORK" strengthens "K" in "WOR_").  
- **Success: Word Superiority Effect**: Letters are easier to recognize in real words ("WORK") than non-words ("OWRK")—top-down feedback boosts letter activation.  

##### 2. COHORT Model (Marslen-Wilson, 1987)  
- **Architecture**: For spoken word access (3 phases):  
  1. **Activation**: Onset sounds (e.g., /kæ/) activate all matching words ("cat," "cap," "can" = cohort).  
  2. **Selection**: Input (new sounds: /kæt/) + context ("The ___ meowed") narrow the cohort to one word ("cat").  
  3. **Integration**: Merge word meaning/grammar into the utterance.  
- **Key Concepts**:  
  - **Recognition Point**: Moment cohort = 1 word (e.g., "trespass" is recognized after /tres/—no other word starts with /tres/).  
  - **Autonomous Activation**: Context can’t block inappropriate cohort members (e.g., /capt/ primes "ship" [captain] and "guard" [captive] even in biasing contexts).  

#### C. Third-Generation (Distributed Representations)  
Neural network-style patterns (not discrete units).  

##### 1. Simple Recurrent Network (SRN; Elman, 2004)  
- **Architecture**: Extends TRACE with a "context layer" to track word order. Trained to predict the next word in sentences.  
- **Outcome**: Hidden unit patterns cluster by part of speech (nouns vs. verbs) and semantics ("cat"/"dog" closer than "cat"/"chair").  

##### 2. Distributed Cohort Model (DCM; Gaskell & Marslen-Wilson, 2002)  
- **Architecture**: Cohort activation + distributed vectors (phonological form + semantic meaning).  
- **Strength**: Explains coarticulation (e.g., "lean" → "leam" before "bacon" due to /n/→/m/); uses sublexical cues (shorter /æ/ in "hamster" vs. longer /æ/ in "ham") to bias correct words.  


## 2. Lexical Ambiguity Resolution  
### 2.1 The Problem  
40% of English words are ambiguous (e.g., "bank" = financial/river; "bug" = insect/listening device). Question: Do we access *all meanings* (exhaustive) or *only contextually appropriate* (exclusive)?  

### 2.2 Key Experiment: Swinney (1979)  
- **Design**: Ambiguous words in biasing contexts (e.g., "The spy looked for concealed bugs" [biases "device"]).  
- **Task**: After "bugs," judge if visual probes ("listen" = device; "insect" = bug; "table" = unrelated) are real words.  
- **Result**:  
  - Short SOA (0 ms): Both "listen" and "insect" are primed (exhaustive access).  
  - Long SOA (250-500 ms): Only the contextually appropriate probe is primed (context suppresses others).  
- **Conclusion**: Exhaustive access first → context filters inappropriate meanings.  

### 2.3 Meaning Dominance & Reordered Access Theory  
Ambiguous words have dominant (frequent) and subordinate (infrequent) meanings (e.g., "tin" = "metal can" [dominant] vs. "bean container" [subordinate]).  

| Ambiguity Type | Neutral Context | Biasing Dominant Meaning | Biasing Subordinate Meaning |  
|----------------|-----------------|--------------------------|-----------------------------|  
| **Balanced** (e.g., "bug") | Slow (competition) | Fast (context resolves) | Fast (context resolves) |  
| **Biased** (e.g., "tin") | Fast (dominant wins) | Fast (no competition) | Slow (subordinate overcomes dominant) |  

- **Eye-Tracking Evidence**: Balanced words (e.g., "bugs") are fixated longer in neutral contexts; biased words (e.g., "tin") are longer only when context favors subordinates.  


## 3. Neural Basis of Lexical Processing  
### 3.1 Core Neuropsychology Observations  
Brain damage shows quasi-independent systems for word form vs. meaning:  
- Some patients define concepts ("skunk = black/white, smells bad") but can’t name the word.  
- Others name words but lack conceptual knowledge (call "skunk" a "cat" and can’t describe its smell).  

### 3.2 Key Brain Regions (Left-Lateralized Network)  
| Processing Type       | Regions                                  | Function                                                                 | Example                                  |
|-----------------------|------------------------------------------|--------------------------------------------------------------------------|------------------------------------------|
| **Auditory Word Form**| Superior temporal lobes (bilateral); Wernicke’s area | Map sound → word form.                                                  | Recognize /kæt/ as "cat".               |
| **Visual Word Form**  | Left fusiform gyrus (visual word form area) | Specialized for pronounceable letter strings (not non-words/pictures).   | Recognize "cat" vs. "cta".               |
| **Semantic Access**   | Inferior temporal lobes; left inferior frontal lobe | Retrieve meaning; integrate with context.                                | Link "cat" to "furry, meows".           |
| **Motor-Language Links** | Motor cortex; mirror neuron system | Simulate actions for action words.                                       | "Throw" activates arm-motor regions.     |

### 3.3 Key Neuroimaging Evidence  
#### A. Action Words & Motor Cortex  
- **fMRI (Hauk et al., 2004)**: "Smile" (face) activates face-motor cortex; "walk" (leg) activates leg-motor cortex—supports embodied semantics.  
- **TMS (Pulvermüller et al., 2005)**: TMS to arm-motor cortex speeds decisions for "lift" (arm-related); TMS to leg-motor cortex speeds "kick" (leg-related).  

#### B. Category-Specific Activation  
- **PET (Martin et al., 1996)**: Naming animals activates occipital (visual) regions; naming tools activates frontal (motor) regions.  
- **Patient Data**: Lesions in left posterior temporal lobe = can’t name tools; anterior temporal lobe = can’t name animals.  

### 3.4 Debate: Localized vs. Distributed Representation  
| View               | Core Claim                                  | Evidence For                                  | Evidence Against                                  |
|--------------------|----------------------------------------------|-----------------------------------------------|---------------------------------------------------|
| **Localized**      | Concepts stored in specific regions (e.g., "tools" = left parietal lobe). | Category-specific deficits (e.g., can’t name animals but can name tools). | - Motor cortex lesions don’t always impair action word understanding.<br>- Landmarks/people both activate left temporal pole (no category split). |
| **Distributed**    | Concepts = activity patterns across networks (e.g., "cat" = visual + auditory + motor regions). | - fMRI shows overlapping but distinct patterns for "cat"/"dog".<br>- Category deficits reflect feature type issues (e.g., animals need fine visual features). | Can’t explain why some lesions only affect one category. |  


## Quick Review Questions  
1. What is the key difference between first- and second-generation lexical access models?  
2. How does the COHORT model explain recognizing "trespass" before the word ends?  
3. What does Swinney’s (1979) study tell us about ambiguity resolution?  
4. Which brain region is specialized for visual word form (e.g., recognizing "cat" vs. "cta")?  
5. How do action words (e.g., "throw") link to motor cortex?



