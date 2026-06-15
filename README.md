# Halanta: A Manually Annotated Dataset for Halanta and ZWNJ Prediction in Nepali

## Overview
This repository contains a manually annotated dataset of 5,000 Nepali sentence pairs created to support 
research on schwa deletion (halanta marking) and Zero-Width Non-Joiner (ZWNJ) insertion in Nepali text. 
The dataset addresses the orthographic–phonological mismatch in Nepali writing, where the inherent vowel 
of consonants is frequently deleted in pronunciation but not consistently marked in standard orthography.

This dataset was developed to support Nepali Text-to-Speech (TTS) systems, grapheme-to-phoneme (G2P) 
conversion, and related NLP research on Nepali phonology.

## Dataset Description

**File:** `gold_halantaV3_Extended.csv`

**Format:** CSV with two columns:

| Column | Description |
|--------|--------------|
| `input` | Original Nepali sentence in standard orthography (no explicit halanta or ZWNJ markers for schwa-deleted consonants) |
| `output` | Phonetically annotated version of the same sentence, with halanta diacritic (्) and Zero-Width Non-Joiner (ZWNJ) characters inserted at positions where schwa deletion occurs, based on phonological rules |

**Size:** 5,000 sentence pairs

**Example:**

| input | output |
|-------|--------|
| आइतवार हप्ताको अन्तिम दिन हो। | आइतवार् हप्ताको अन्तिम् दिन् हो। |
| म हरेक दिन भात खान्छु। | म हरेक् दिन् भात् खान्छु। |
| उपहारको लागि टमलाई धन्यवाद दिन सम्झनुहोस्। | उपहार्‌को लागि टम्‌लाई धन्यवाद् दिन सम्झनुहोस्। |

## Annotation Methodology
Annotations were performed manually according to established phonological rules for:
- Schwa deletion in word-final and word-medial consonants
- Conjunct consonant formation
- Morpheme boundary identification (marked using ZWNJ where applicable)

## Intended Use
This dataset is intended for:
- Training and evaluating sequence-to-sequence models for halanta/ZWNJ prediction
- Grapheme-to-phoneme (G2P) conversion research for Nepali
- Nepali Text-to-Speech (TTS) front-end development
- Linguistic research on Nepali orthography–phonology mismatch

## Citation
If you use this dataset, please cite:

> [Citation details to be added upon publication]

## License
This dataset is released under the [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/) license. 
You are free to share and adapt the data for any purpose, provided appropriate credit is given.

## Contact
For questions regarding this dataset, please open an issue in this repository.
