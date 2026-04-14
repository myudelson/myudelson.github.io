---
name: "Optimizing delivery of educational content in the era of Big Data"
title: "Optimizing delivery of educational content in the era of Big Data"
layout: talk
date: June 9, 2017
description: "Invited seminar at the School of Higher Mathematics and Cybernetics of Moscow State University, Russia."
tags: [Educational Data Mining, Data Science, Big Data]
image: ../assets/img/msk-2017-msu-vmk-talk.jpg
---

>Audience: students, faculty.

## Architectural Resilience and Component-Based Adaptivity

State-of-the-art adaptive learning environments are no longer monolithic entities but are defined by a sophisticated, decoupled architecture comprising learning management portals, content delivery servers, and centralized user model servers. This modularity allows for "value-added services" and adaptive shells to be integrated via plugins or thin-client engines, such as the PERSEUS adaptation engine, which replaces manual programming with configuration-based deployment. By separating user statistics and knowledge modeling from the delivery of educational content, these systems achieve the scalability required to support diverse pedagogical domains – from SQL and Java programming to cognitive algebra tutors – while maintaining the flexibility to evolve without systemic overhauls.

## Advancements in Large-Scale Student Knowledge Modeling

The core of modern computer-aided support lies in the ability to track student knowledge transitions through Bayesian Knowledge Tracing (BKT) and Additive Factor Models (AFM). Leveraging "Big Data" from massive open online courses (MOOCs) and cognitive tutors, these models utilize EM-algorithms and logistic regression with random effects to predict student performance and identify learning plateaus. Recent breakthroughs include the development of high-performance, open-source utilities (e.g., hmm-scalable and modified LIBLINEAR) capable of processing billions of data points across tens of thousands of concepts and students, effectively shifting the bottleneck from computational capacity to the refinement of cognitive models.


## Automated Concept Extraction and the Limits of Stereotyped Adaptation

In unstructured environments like programming MOOCs, where manual concept mapping is unfeasible, state-of-the-art methods now employ automated parsing of source code to extract latent concepts directly from abstract syntax trees. While these automated AFM models demonstrate high predictive accuracy (up to 75%) and practical utility in generating real-time coding prompts, research indicates a significant challenge in stereotyped adaptation. Current evidence suggests that segmenting students into groups based on demographics or broad behavioral clusters (e.g., "strugglers" vs. "builders") does not yield significantly different or more effective knowledge models. This suggests that future adaptive strategies must move toward localized, moment-to-moment behavioral analysis rather than static student profiles to truly optimize the individual learning trajectory.

> Drafted with AI assistance and reviewed for accuracy 🤖

## Slides

Attached slides are in Russian.

<iframe
  src="{{ '/assets/pdfjs/web/viewer.html?file=' | append: '/assets/pdf/slides/msk-2017-msu-vmk-talk.pdf' | absolute_url }}"
  width="80%"
  height="600px"
  style="border:none;">
</iframe>

