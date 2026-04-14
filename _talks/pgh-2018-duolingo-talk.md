---
name: "Better Data Beats Big Data: A Case of Education"
title: "Better Data Beats Big Data: A Case of Education"
layout: talk
date: June 21, 2018
description: "Invited talk at Duolingo headquarters in Pittsburgh, PA, USA."
tags: [Big Data, Educational Data Mining]
image: ../assets/img/pgh-2018-duolingo-talk-tall.jpg
---

>Audience: professionals, educators.

## The Fallacy of Computational Brute Force

While the emergence of Big Data and data science has fostered the belief that population-scale datasets inherently produce more generalizable models, this research posits that not all data is created equal. In the context of educational modeling, specifically for the Carnegie Learning Cognitive Tutor Algebra (CTA) platform, the study demonstrates that "more" does not necessarily equate to "better". Instead, a curated fraction of educational data can effectively represent the full dataset, suggesting that ML strategies should pivot from indiscriminate data ingestion to the identification of high-fidelity subsets. For executives, this highlights a critical efficiency: reducing the noise in "Big Data" through selective inclusion can lead to more robust, actionable student models without the overhead of processing low-quality signals.

## Identifying High-Utility Data Segments

The research explored whether external metadata – such as school locale, size, or socioeconomic status (SES) – could serve as effective grouping factors for tuning models. Interestingly, traditional demographic markers like school locale and student-teacher ratios proved non-significant for predictive accuracy. The most impactful "Better Data" came from internal usage metrics and model-derived values, specifically average student units attempted and skill intercept/slope parameters. This suggests that behavioral dedication and engagement are superior predictors compared to static demographic data. By clustering schools based on these performance-centric factors, the study found a "cleanly separated" group of high-usage schools that effectively represented the optimal training set for the broader population.

## Operational Implications: Curation as a Competitive Advantage

The findings support a "working hypothesis" that data quality is a function of user dedication. Schools with larger enrollments or lower SES often exhibited lower dedication to the tutor, resulting in "bad" data that significantly degraded model performance. Consequently, an effective ML strategy for the C-suite involves selective data admission: prioritizing data from "established" users who meet recommended usage thresholds (e.g., 48 hours per semester). By being selective rather than inclusive, organizations can build models that are not only more accurate but also more reflective of the learning objectives the technology was designed to achieve

> Drafted with AI assistance and reviewed for accuracy 🤖

## Slides

<iframe
  src="{{ '/assets/pdfjs/web/viewer.html?file=' | append: '/assets/pdf/slides/pgh-2018-duolingo-talk.pdf' | absolute_url }}"
  width="80%"
  height="600px"
  style="border:none;">
</iframe>

