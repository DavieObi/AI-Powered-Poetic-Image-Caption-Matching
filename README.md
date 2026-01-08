---

# Aesthetic Image–Text Alignment for Poetic Caption Recommendation

## Overview

This project explores **aesthetic and emotional alignment between images and text** using a multimodal machine learning approach. Instead of generating literal descriptions of an image, the system recommends **poetic, mood-driven captions** that *feel right* for the image — similar to how captions are chosen for social media platforms like Instagram.

The core question this project answers is not:

> *“What is in the image?”*

but rather:

> **“What does this image feel like?”**

Using a pretrained vision–language model, the system evaluates how well a set of candidate captions semantically aligns with an image and ranks them based on similarity.

---

## Motivation

Traditional image captioning focuses on object detection and factual descriptions. While useful for accessibility and search, this approach does not reflect how images are commonly used in creative or social contexts.

On platforms like Instagram, captions are often:

* poetic
* reflective
* emotional
* abstract
* story-driven

This project was designed to bridge that gap by applying **semantic image–text similarity** to recommend captions that match an image’s *mood*, not just its content.

---

## Core Idea

The system embeds:

* an image, and
* a list of candidate captions

into a **shared semantic space**, then measures how closely each caption aligns with the image.

The output is a ranked list of captions, ordered by semantic similarity.

Key characteristics:

* Captions are **not generated**
* Captions are **selected** from a predefined set
* Ranking is based on **conceptual alignment**, not keywords

---

## Process Overview: From Literal Description to Poetic Alignment

### Step 1: Validating Literal Image–Text Matching

The project began by validating the technical pipeline using **literal, descriptive captions** that explicitly referenced visible elements in the image (e.g., people, walkways, greenery, buildings).

This step ensured that:

* Image embeddings were generated correctly
* Text embeddings shared the same semantic space
* Cosine similarity produced meaningful rankings

Once this baseline was confirmed, the focus shifted from correctness to creativity.

---

### Step 2: Reframing the Objective

Rather than asking:

> *“What does this image show?”*

The objective was reframed to:

> **“What emotion or atmosphere does this image convey?”**

At this stage:

* All candidate captions were rewritten to be **poetic and mood-based**
* Captions avoided naming objects, locations, or actions
* Emphasis was placed on emotion, symbolism, and interpretation

This reframing mirrors real-world captioning behavior on social media.

---

### Step 3: Poetic Caption Selection via Semantic Similarity

The system then evaluated how well each poetic caption semantically aligned with the image.

Although these captions do not describe visible elements directly, the model associates abstract language with visual cues such as:

* calm pedestrian movement
* greenery within urban infrastructure
* quiet transitions
* everyday journeys

---

## Results and Interpretation

### Top Ranked Captions

```
1. Where concrete learns to coexist with green. (0.2616)
2. A pause in the rush of the city. (0.2505)
3. The city breathes when you slow down. (0.2292)
4. Moving forward, quietly. (0.2143)
5. Every step has a story. (0.2128)
```

### What These Results Show

#### Conceptual Over Literal Alignment

The highest-ranked caption — *“Where concrete learns to coexist with green.”* — reflects strong conceptual overlap between the image and the text.

Without describing any objects explicitly, it aligns with:

* visible greenery
* surrounding urban structures
* the balance between nature and city life

This demonstrates that the system captures **abstract relationships**, not just object-level features.

---

#### Mood and Atmosphere Recognition

Captions such as *“A pause in the rush of the city”* and *“The city breathes when you slow down”* score highly because the image conveys:

* calm, unhurried movement
* absence of visual chaos
* a reflective urban atmosphere

The similarity rankings confirm that the model recognizes emotional tone, not just visual content.

---

#### Interpreting Similarity Scores

Poetic captions naturally yield **lower similarity scores** than literal descriptions. This is expected and not a limitation.

Reasons include:

* Abstract language has fewer direct visual anchors
* Emotional interpretation is inherently broader
* Multiple captions may be equally valid

In this context, **relative ranking** is more meaningful than absolute score values.

---

## What This Project Is (and Is Not)

### This project **is**:

* A multimodal image–text alignment system
* Focused on mood, tone, and aesthetic interpretation
* Suitable for creative and social media use cases
* An application of pretrained vision–language models

### This project **is not**:

* A traditional image caption generator
* An object detection or labeling system
* A fine-tuned or custom-trained model
* Designed for accessibility or factual annotation

---

## Potential Applications

* Instagram caption recommendation
* Creative writing inspiration
* Visual storytelling tools
* Mood-based content curation
* AI-assisted lifestyle and photography platforms

---

## Limitations

* Output quality depends heavily on the quality of candidate captions
* Cultural and emotional interpretation can vary
* The system does not generate new captions
* Abstract alignment is subjective by nature

---

## Key Takeaway

This project demonstrates that multimodal AI can be used not only for *describing* the world, but also for *interpreting* it.

By shifting from literal captions to poetic alignment, the system reflects how humans naturally engage with images in creative contexts.

---

## Author

**David Obi**
Data Scientist | Machine Learning Engineer
Focused on practical, creative, and human-centered AI applications

---
