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

Key characteristics:

* Captions are **not generated**
* Captions are **selected** from a predefined set
* Ranking is based on **conceptual alignment**, not literal description

---

## Process Overview

### Step 1: Validating Literal Alignment

The project began by validating the pipeline using literal, descriptive captions to confirm that image–text similarity was working correctly.

This ensured:

* Image embeddings were generated correctly
* Text embeddings shared the same semantic space
* Similarity ranking behaved as expected

---

### Step 2: Shifting to Poetic Intent

Once validated, the objective was reframed from literal description to emotional interpretation.

Instead of asking:

> *“What does this image show?”*

The system asks:

> **“What emotion or atmosphere does this image convey?”**

At this stage:

* Captions were rewritten to be poetic and abstract
* Object names and literal references were removed
* Emphasis was placed on mood, reflection, and storytelling

---

### Step 3: Poetic Caption Selection

The system evaluates how well each poetic caption aligns with the image using semantic similarity.

Even without direct visual references, the model associates abstract language with:

* calm movement
* urban stillness
* greenery within infrastructure
* everyday transitions

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

### Interpretation

* The highest-ranked captions reflect **conceptual and emotional alignment**, not object recognition.
* Lower similarity scores are expected for poetic text and do not indicate poor performance.
* Ranking order is more meaningful than absolute values.

These results show that multimodal models can capture **aesthetic and emotional signals**, not just literal content.

---

## What This Project Is (and Is Not)

### This project is:

* A multimodal image–text alignment system
* Focused on mood, tone, and interpretation
* Suitable for creative and social media use

### This project is not:

* A traditional image caption generator
* An object detection system
* A fine-tuned or custom-trained model

---

## Potential Applications

* Instagram caption recommendation
* Creative writing inspiration
* Visual storytelling tools
* Mood-based content curation

---

## Key Takeaway

This project demonstrates that multimodal AI can be used not only for describing images, but also for interpreting them in creative and human-centered ways.

---

## Author

**David Obi**
Data Scientist | Machine Learning Engineer
