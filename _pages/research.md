---
layout: page
permalink: /research/
title: research
description: Brief descriptions on what I am working on and what interests me!
nav: true
---

<a name="toc"></a> I am a strong proponent of collaborative research work. Throughout my research experience (so far, much more to go!), I am extremely fortunate to have found supportive mentors and amazing collaborators. I thank them for the opportunities and advice, as none of these projects would've been possible without them! If you have thoughts/comments on any of the projects I am currently working on, I'd love to hop on a quick call to chat about them! 

# Table of Contents 
- [What am I working on right now?](#current)
    - [Refining LMs via human-in-the-loop explanations](#current-first)
    -  [Implicit concept-driven model explanations](#current-second)
- [Other Research Interests](#interests)
- [Past Work and Side Projects](#past)
    - [Social Networks](#sn)
    - [Music and Machine Learning](#mml)

### **What am I working on right now?** <a name="current"></a> [⬆️](#toc)

#### Refining LMs via human-in-the-loop explanations 🤖 ➡ 👧🏾 ➡ 🤖 <a name="current-first"></a>

In this project, our team ([Aaron Chan](https://aarzchan.com/), Ziyi Liu and [Prof. Xiang Ren](https://shanzhenren.github.io/)) aims to “close the loop” between generating and utilizing explanations. We believe that LM explanations should not just be used to passively interpret LM behavior, but rather operationalized to actively improve how LMs make decisions. 

To this end, we are exploring (human-in-the-loop) HITL interventions to identifying spurious patterns in model explanations, and further utilising these intervention to regularise LMs to effectively debug them and potentially improve their performance in selected scenarios. More specifically, we are interested in the following **research questions**:

1. How can human annotators efficiently intervene model explanations, with given *time constraints*?
2. How can we present samples to human annotators so that we can gain maximum benefit out of them? (Like generalising to more samples, by intervening only on candidate samples)
3. How can interventions provided by human annotators be utilised by LMs to regularise/tune them accordingly?
4. How do these interventions help in improving model performance and fixing spurious patterns in the long run?

#### Implicit concept-driven model explanations 🧠 ➡ 📖 <a name="current-second"></a>

In another exploratory project, I am expounding upon current development in concept oriented model explanations (like [Koh et. al, 2020](https://arxiv.org/abs/2007.04612)). These methods extract human-readable abstractions called *concepts* from either model predictions or intermediate layers, which serve as key indicators of model behaviour. These *concepts* often serve as a proxy for model explanations, as they are used *within* the model for prediction, rather than post-hoc approaches.

However, for textual domains, often these concept are implicit -- not present in the surface form in the text, but prior-knowledge informed. I aim to identify these implicit concepts as model explanations. More on this idea later!

### **Other Research Interests** <a name="interests"></a> [⬆️](#toc)

Very broadly, I am interested in working on problems around developing **label-efficient** methods for NLP tasks (brownie points to the project if they are for developing **explainable** and/or **robust** systems). That said, I am open to exploring other ideas (hmu if you want to collaborate!)

Some stuff that I found interesting and would like to explore in the future:

1. **Demystifying model explanations via human-interactions**: Lately, I have been very interested in understanding the degree to which explanations align with human-perceived notions. [Schuff et. al, 2022](https://arxiv.org/abs/2201.11569) provide interesting insights on how humans often mis-interpret saliency-based explanations and suggest approaches to mitigate it. [Krishna et. al, 2022](https://arxiv.org/pdf/2202.01602.pdf) conduct an extensive user study to formalise disagreements caused by several model explanation methods. [Adebayo et. al, 2022](https://openreview.net/forum?id=xNOVfCCvDpM) also explore whether model explanations are enough to identify spurious signals via user studies.

2. **Utilising explanations to identify and calibrate model behaviour**: I am particularly interested in using model explanations in ways that can underscore potential bias or model leakage in sensitive scenarios. I particularly like approaches like that used by [Kennedy et. al, 2020](https://arxiv.org/abs/2005.02439), which employ explanations to identify cases where models overly rely on sensitive attributes like race, gender, etc, rather than focusing on the context surrounding them in hate speech. I am also interested in approaches that can explain moral dilemmas (for improving blackbox systems like [Delphi](https://delphi.allenai.org/)) or identify model leakage, specifically in sensitive scenarios like clinical data, as shown by [Lehman et. al, 2021](https://arxiv.org/abs/2104.07762).

### **Past Work and Side Projects** <a name="past"></a> [⬆️](#toc)

#### Social Networks <a name="sn"></a>

In what I consider past life now 😄, I spent considerable time working on topics in anomaly detection on social networks like Twitter. As a part of 2 year long undergraduate thesis work, I worked on a novel problem of *collusion detection*, where malicious entities come together to trade appraisals on social media platforms. Along with my team members [Aditya Chetan](https://justachetan.github.io/), [Dr. Hridoy Sankar Dutta](https://hridaydutta123.github.io/) and [Prof. Tanmoy Chakraborty](https://faculty.iiitd.ac.in/~tanmoy/), we worked on a series of projects surrounding Collusion detection:

1. In a preliminary study [(ASONAM'18)](https://arxiv.org/abs/1806.08979), we established the differences between collusion detection and bot/spam detection methods, followed by a supervised, feature-based classification system to identify collusive retweeters over Twitter. This was an important work to *actively probe* collusive users and collect labelled data in that manner, along with identifying characteristics pertaining to their behaviour.

2. In a follow up work [(WSDM'19)](https://dl.acm.org/doi/10.1145/3289600.3291010), we devised an unsupervised approach in identifying collusive users, owing to the scarcity of labelled data. We made use of a *learning-to-rank* approach, coupled with features that were intrinsic to collusive behaviour. I am extremely proud of this work, particularly because everything from approach design to implementation was conducted by a bunch of undergrads (my collaborator Aditya and I), and provided me with the necessary motivation to pursue a PhD! 🙌🏽

3. In a spin-off project [(ACM TIST)](https://dl.acm.org/doi/abs/10.1145/3380537) of the first work, [Udit Arora](https://uditarora.com/) and our team designed a *multi-view* approach to looking at collusive users -- from a follower/followee, tweet and content perspective, to enrich the signals for effective classification.

#### Music and Machine Learning <a name="mml"></a>

I have also dabbled with a diverse set of problems in music (audio) and machine learning. Some problems that I have worked on:

1. What are the textual ingredients necessary to make a podcast popular? [(NLP4MusA)](https://aclanthology.org/2020.nlp4musa-1.3/)

2. Understanding the difference between emotions conveyed and induced by hindustani classical music. [(ICMI'20 Late Breaking Reports)](https://dl.acm.org/doi/abs/10.1145/3395035.3425246)

3. Beatbox transcription to symbolic notations: from generating a diverse dataset to a first approach in solving this task. [(PAKDD'22)]()

