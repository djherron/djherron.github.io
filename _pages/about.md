---
layout: about
title: about
permalink: /
subtitle: student @ City St George's, University of London, London, UK

profile:
  align: right
  image: me.jpg
  image_circular: false # crops the image to make it circular
  more_info: >

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit:  # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I'm a PhD student of artificial intelligence. My research focuses on **neurosymbolic learning and reasoning with OWL-based knowledge graphs**.  

**Neurosymbolic AI** explores the blending of the neural (connectionist) AI tradition with the symbolic AI tradition in order to get the best of both worlds. **Neural AI** (deep learning with neural networks) uses **inductive learning** (learning from examples) to **learn subsymbolic features** from data. **Symbolic AI** uses **symbolic representations of knowledge** and logical inference techniques (both based on logical formalisms) to do **symbolic deductive reasoning**. Neural AI has a **statistical** character; symbolic AI has a **logical** character. These differences in character make blending these two traditions of AI, in hybrid neurosymbolic systems, challenging.

My research uses **Semantic Web** technologies for the symbolic components of neurosymbolic systems.  More specifically, I explore using **OWL-based knowledge graph technologies**, **OWL ontologies**, and **OWL reasoning** for the symbolic components of neurosymbolic systems.

OWL (the Web Ontology Language) is the Semantic Web's language for defining **ontologies** (formal descriptions of domains of interest). OWL is the W3C Web-friendly version of the **Description Logic** named $\mathcal{SROIQ}$. An OWL ontology thus has associated **inference semantics** that permit **sound and complete logical inference** to be performed via OWL reasoning tools.

My research explores the question of how to **combine subsymbolic (deep) learning with symbolic (OWL) reasoning** in neurosymbolic systems.

#### Knowledge graph reasoning for visual relationship detection

One thread of my research uses the computer vision task of **visual relationship detection** (VRD) within images as the context for exploring this question. I consider various approaches to leveraging various OWL reasoning capabilities so as to guide and improve subsymbolic learning. The effects of the symbolic OWL reasoning on subsymbolic learning are examined by evaluating the predictive performance of neurosymbolic VRD systems. The performance they exhibit is compared with the performance exhibited by corresponding baseline VRD systems trained using deep learning only, unaided by auxiliary symbolic OWL reasoning in any way.

This thread of my research expands perceptions of Semantic Web and OWL-based knowledge graph technologies by demonstrating them being leveraged in a novel use case: that of **symbolic reasoning engines in neurosymbolic systems**. An OWL-based knowledge graph tool acts as the engine, and an OWL ontology is used in a manner akin to a **logic program**.  The engine hosts the OWL ontology. It represents an OWL-based knowledge graph empty of any data facts. The ontology governs what OWL reasoning can and cannot do when the engine (the knowledge graph) is presented with data facts. The engine is only ever presented with one 'tiny world' of data facts at a time, but in rapid succession, as driven by the demands of a neural network training cycle or inference cycle. The results (feedback) of the engine's symbolic OWL reasoning are then used to guide subsymbolic learning and/or inference. These results may take the form of newly inferred data facts or detection of logical inconsistencies.

#### Tensor knowledge graphs

Another thread of my research explores and develops my concepts of **tensor knowledge graphs**, **tensor knowledge graph reasoning**.

A conventional OWL-based knowledge graph has a directed graph representation consisting of a collection of text-based RDF triples. A **tensor knowledge graph** represents the same symbolic knowledge (without loss of information) using **binary relations represented as Boolean matrices**. Binary relation matrices of like size are collected into 3D Boolean tensors, with each matrix occupying a distinct *channel* of a particular 3D tensor.  The tensors of a tensor knowledge graph are strictly Boolean, and hence the knowledge they represent is strictly symbolic, just like in a conventional (directed graph) OWL-based knowledge graph.

**Tensor knowledge graph reasoning** seeks to emulate conventional (directed graph) OWL reasoning. The techniques I'm developing for performing OWL-based logical inference on tensor knowledge graphs rely entirely upon the tensor knowledge graph representation of the symbolic knowledge of a knowledge graph. That is, my tensor knowledge graph reasoning techniques are based on **Boolean algebra applied to the Boolean matrices that encode the binary relations of a knowledge graph**.  The reasoning techniques rely only upon matrix-based implementations of **binary relational operations**, and upon vector-based implementations of **set operations**. My tensor knowledge graph reasoning techniques represent a new category of approach to OWL reasoning, and, more broadly, to Description Logic reasoning generally.  My approach is grounded in relational mathematics (binary relation theory) and set theory, as are all Description Logics.


#### Tensor knowledge graph applications in neurosymbolic systems

A further thread of my research explores applications of tensor knowledge graphs, and tensor knowledge graph reasoning, in neurosymbolic systems.

A key application involves implementing tensor knowledge graphs and tensor knowledge graph reasoning within a **tensor knowledge graph reasoning engine**. This is a software tool whose target use case is **symbolic reasoning engine** components in neurosymbolic systems.  The engine's API, and the services it exposes, are tailored for use by neurosymbolic researchers in neurosymbolic systems, based on my experience using conventional (directed graph) OWL-based knowledge graph technologies in the 'KG reasoning for visual relationship detection' thread of my research.


