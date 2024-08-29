---
title: "Can Visual Language Models Replace OCR-Based Visual Question Answering Pipelines in Production? A Case Study in Retail."
collection: publications
permalink: /publication/ECCV24_EVAL-FoMo_Workshop
excerpt: 'Most production-level deployments for Visual Question Answering (VQA) tasks are still build as processing pipelines of independent steps.
However, the recent advances in vision Foundation Models [25] and Vision Language Models (VLMs) [23] raise the question if these custom trained, multi-step approaches can be replaced with pre-trained, single-step VLMs. This paper analyzes the performance and limits of various VLMs in the context of VQA and OCR [5, 9, 12] tasks in a production-level scenario. In conclusion, the VQA task which aims to predict specific product information from images being satisfying but performs less fulfilling in identifying specific features, possibly due to a lack of domain-specific knowledge.'
date: 2024-08-29
venue: Emergent Visual Abilities and Limits of Foundation Models Workshop, ECCV 2024, Milan
paperurl: 'https://arxiv.org/pdf/2408.15626'
---
Most production-level deployments for Visual Question Answering (VQA) tasks are still build as processing pipelines of independent steps including image pre-processing, object- and text detection, Optical Character Recognition (OCR) and (mostly supervised) object classification. However, the recent advances in vision Foundation Models [25] and Vision Language Models (VLMs) [23] raise the question if these custom trained, multi-step approaches can be replaced with pre-trained, single-step VLMs.
This paper analyzes the performance and limits of various VLMs in the context of VQA and OCR [5, 9, 12] tasks in a production-level scenario. Using data from the Retail-786k [10] dataset, we investigate the capabilities of pre-trained VLMs to answer detailed questions about advertised products in images. Our study includes two commercial models, GPT-4V [16] and GPT-4o [17], as well as four open-source models: InternVL [5], LLaVA 1.5 [12], LLaVA-NeXT [13], and CogAgent [9].
Our initial results show, that there is in general no big performance gap between open-source and commercial models. However, we observe a strong task dependent variance in VLM performance: while most models are able to answer questions regarding the product brand and price with high accuracy, they completely fail at the same time to correctly identity the specific product name or discount. This indicates the problem of VLMs to solve fine-grained classification tasks as well to model the more abstract concept of discounts.

[Download paper here](https://arxiv.org/pdf/2408.15626)