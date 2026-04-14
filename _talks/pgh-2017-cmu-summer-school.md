---
name: "Bayesian Knowledge Tracing at Scale woth HMM Scalable toolkit"
title: "Bayesian Knowledge Tracing at Scale woth HMM Scalable toolkit"
layout: talk
date: July 2017
description: "Invited lecture at the 2017 LearnLab Summer School, Carnegie Mellon University."
tags: [Summer School, Data Science, Educational Data Mining]
image: ../assets/img/pgh-2017-cmu-summer-school.png
---

>Audience: students, faculty, professionals.

This talk presemts **hmm-scalable**  a highly-capable tool for fitting Bayesian Knowledge Tracing (BKT), a specialized form of Hidden Markov Modeling used in the fields of Computer-Assisted Learning and Intelligent Tutoring Systems to optimize learning outcomes.

## Bayesian Knowledge Tracing

Bayesian Knowledge Tracing is a computational framework specifically designed to model a student’s mastery of individual skills over time. At its core, BKT is a **Hidden Markov Model (HMM)** characterized by two binary variables:

* **Latent Variable (Mastery):** An unobserved state representing whether a student "knows" or "does not know" a skill.
* **Observed Variable (Performance):** The recorded success or failure of a student on a specific problem step.

The model transitions between these states based on four primary parameters: **pInit** (initial knowledge), **pLearn** (probability of moving from unlearned to learned), **pGuess** (probability of a correct answer despite lack of mastery), and **pSlip** (probability of an error despite mastery). By treating student performance as a time-series of these transitions and emissions, BKT allows "Cognitive Mastery" systems to strategically deliver content only for unmastered skills.

### Scaling to Big Data with hmm-scalable

While BKT is conceptually powerful, fitting these models to massive datasets – such as those from large-scale Intelligent Tutoring Systems – requires significant computational efficiency. The **hmm-scalable** toolkit is a specialized software package built to handle "Big Datasets" that may contain hundreds of millions of records and over 100,000 students.

The tool's impact is most evident in its processing speed:

*  **Performance:** It can fit a 20-million-record dataset (like the KDD Cup 2010 challenge) in approximately one minute.
* **Efficiency:** Even a synthetic dataset of close to a **billion million records** can be processed in roughly 20 minutes using the tool's multi-core parallel execution mode.
* **Parallelization:** The toolkit utilizes **Open MP** to fit individual skills in parallel threads, reducing processing time from over two minutes to approximately 33 seconds on standard hardware.

### Suite of Optimization Solvers

Beyond mere speed, **hmm-scalable** provides several _solvers_ to refine model accuracy, which directly affects student learning efficiency. Users can choose between the classical **Baum-Welch (EM)** algorithm, **Stochastic Gradient Descent**, and various **Conjugate Gradient Descent** methods. These solvers allow for the exploration of complex BKT variants, such as **Individualized BKT**, which accounts for student-specific variations in performance.

The choice of solver and model precision is not merely technical; it is pedagogically significant. For example, a model that more accurately predicts a higher **pLearn** value allows a student to reach the mastery threshold faster, resulting in fewer required problems and reduced total instructional time. Ultimately, **hmm-scalable** serves as the bridge between theoretical HMM research and the practical, high-speed demands of modern educational technology.

> Drafted with AI assistance and reviewed for accuracy 🤖

## Slides

<iframe
  src="{{ '/assets/pdfjs/web/viewer.html?file=' | append: '/assets/pdf/slides/2017_CMU_LearnLab_SummerSchool_HMM-scalable.pdf' | absolute_url }}"
  width="80%"
  height="600px"
  style="border:none;">
</iframe>

