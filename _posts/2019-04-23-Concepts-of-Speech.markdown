---
layout: post
title:  "BASIC CONCEPTS OF SPEECH"
# date:   2018-9-23 23:45:13 +0700
subtitle: "People rarely understand how it is produced and perceived. Speech is a dynamic process without clearly distinguished parts."
author: vocong25
background: ''
tags: [speech, concepts]
# comments: true
---


# BASIC CONCEPTS OF SPEECH

- Structure of Speech
- Models
- Other used concepts
- What is optimized

--- 

**Speech is a complex phenominon.** People rarely understand how it is produced and perceived. Speech is a dynamic process without clearly distinguished parts.

---
## Structure of speech

- Phones: The way to sound a word or a character.

- Diphones: Parts of phones between two consecutive phones.

- Triphones: A phone in a particular context. Example: "n" in the left "ba" is different to "d" in "ba"

- Senones: A detector to detect triphones. A senones's dependence on context can be more complex than just the left and right context. It can be a rather complex function defined by a decision tree, or in some other ways.

- Phone build subword units, like syllables[2]. Sometimes, syllables are defined as "reduction-stable entities". *For instance, when speech becomes fast, phones are often changed, but syllables remain the same.*

- Subwords form words.

## Models

- **An Acoustic Model**: contains acoustic properties for each senone. There are context-independent models that contain properties (the most probable feature vectors for each phone) and context-dependent ones (built from senones with context).

- **A Phonetic Dictionary**: contains a mapping from words to phones. This mapping is not very effective.

- **A Language Model**: is used to restrict word search. It defines which word could follow previously recognized words (matching is a sequential process) and helps to significantly restrict the matching process by stripping words that are not probable.

- **The Vocoder**: (short for voice encoder) is a synthesis system, which was initially developed to reproduce human speech. Vocoding is the cross synthesis of a musical instrument with voice. It was called the vocoder vecause it involved encoding the voice (speech analysis) and then reconstructing the voice in accordance with a code written to replicate the speech (speech synthesis).[3]

## What is optimized

1.  Word error rate (in speech recognition) 

    $$WER=\frac{I + D + S}{N}$$

    ```
    Where: 
        - I is the number of inserted words.
        - D is the number of deleted words.
        - S is represent the number of subtituted words.
    ```

2. Accuracy

    $$acc = \frac{N - D - S}{N}$$

3. Speed

    Suppose an audio file has recording time of 2 hours and then decoding took 6 hours then the speed is counted as 3xreal-time.

4. ROC curve

## Reference

1. `https://cmusphinx.github.io/wiki/tutorialconcepts/?fbclid=IwAR09IrdKhpcCNQ-ayVmCuUa8aQ7jBAdhkMlYsY4SZapgUOAyPC7zduHPK24`

2. `https://writingexplained.org/grammar-dictionary/syllable`

3. `https://ses.library.usyd.edu.au/bitstream/2123/8296/2/311107435%20Technology%20Review%20-%20Vocoder.pdf`

---

## Vocabularies:

1. utterance: 
    - A spoken word, statement, or vocal sound
    - An uninterrupted chain of spoken or written language.

