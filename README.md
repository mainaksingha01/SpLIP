# Elevating All Zero-Shot Sketch-Based Image Retrieval Through Multimodal Prompt Learning (ECCV'24)

Official repository of SpLIP, which introduces a novel multimodal prompting learning (MPL) approach in vision-language models for sketch-based image retrieval tasks.

[![arXiv](https://img.shields.io/badge/arXiv-Paper-brightgreen)](https://arxiv.org/pdf/2407.04207)
[![project](https://img.shields.io/badge/Project-Page-darkred)](https://mainaksingha01.github.io/SpLIP/)

## Abstract
<img src="https://github.com/mainaksingha01/SpLIP/blob/master/static/images/teaser.png" width="1000">

We address the challenges inherent in sketch-based image retrieval (SBIR) across various settings, including zero-shot SBIR, generalized zero-shot SBIR, and fine-grained zero-shot SBIR, by leveraging the vision-language foundation model CLIP. While recent endeavors have employed CLIP to enhance SBIR, these approaches predominantly follow uni-modal prompt processing and overlook to exploit CLIP's integrated visual and textual capabilities fully. To bridge this gap, we introduce SpLIP, a novel multi-modal prompt learning scheme designed to operate effectively with frozen CLIP backbones. We diverge from existing multi-modal prompting methods that treat visual and textual prompts independently or integrate them in a limited fashion, leading to suboptimal generalization. SpLIP implements a bi-directional prompt-sharing strategy that enables mutual knowledge exchange between CLIP's visual and textual encoders, fostering a more cohesive and synergistic prompt processing mechanism that significantly reduces the semantic gap between the sketch and photo embeddings. In addition to pioneering multi-modal prompt learning, we propose two innovative strategies for further refining the embedding space. The first is an adaptive margin generation for the sketch-photo triplet loss, regulated by CLIP's class textual embeddings. The second introduces a novel task, termed conditional cross-modal jigsaw, aimed at enhancing fine-grained sketch-photo alignment by implicitly modeling sketches' viable patch arrangement using knowledge of unshuffled photos. Our comprehensive experimental evaluations across multiple benchmarks demonstrate the superior performance of SpLIP in all three SBIR scenarios.

## Architecture

<img src="https://github.com/mainaksingha01/SpLIP/blob/master/static/images/architecture.png" width="800">
