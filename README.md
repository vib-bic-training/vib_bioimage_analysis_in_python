<!--
author:   Pavie Benjamin
email:    benjamin.pavie@vib.be
version:  1.0.0
language: en
narrator: UK English Male

icon:     https://vib.be/sites/vib.sites.vib.be/files/logo_VIB_noTagline.svg

comment:  This document shall provide an entire compendium and course on the
          development of Open-courSes with [LiaScript](https://LiaScript.github.io).
          As the language and the systems grows, also this document will be updated.
          Feel free to fork or copy it, translations are very welcome...

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js
          https://felixhao28.github.io/JSCPP/dist/JSCPP.es5.min.js

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css
link:     https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
link:     https://raw.githubusercontent.com/vib-tcp/material-liascript/master/img/org.css
link:     https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.min.css
link:     https://fonts.googleapis.com/css2?family=Saira+Condensed:wght@300&display=swap
link:     https://fonts.googleapis.com/css2?family=Open+Sans&display=swap

link:  https://raw.githubusercontent.com/vib-tcp/material-liascript/master/vib-styles.css

@edition:  1st 
@CourseTitle: replace by course title

import:   https://raw.githubusercontent.com/vib-tcp/training_material_template/refs/heads/main/macro.md

-->

# @Bioimage Analysis in Python

<section>

Hello and welcome to our Bioimage Analysis in Python Course

This is the @edition edition of this workshop, organised by VIB.

> We are using the interactive Open Educational Resource online/offline course infrastructure called LiaScript.
> It is a distributed way of creating and sharing educational content hosted on github.
> To see this document as an interactive LiaScript rendered version, click on the
> following link/badge: [LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/vib-bic-training/vib_bioimage_analysis_in_python/main/README.md)

## General context

Microscopy generates complex, multi-dimensional image data that requires efficient analysis to extract meaningful biological insights. This introductory course provides researchers with practical skills for handling and processing microscopy images using Python. 

Participants will learn to visualize, manipulate, and analyze image data using tools such as **Napari**, enabling them to explore 2D and 3D datasets interactively.

The training is designed for early-career scientists and support staff who want to integrate computational approaches into their imaging workflows.

By the end of the session, attendees will be able to perform essential tasks, including **image segmentation**, **metadata handling**, and **quantitative analysis**, laying the foundation for reproducible, automated image processing in research.

## Proposed Schedule

Schedule day 1:

- 9:30 - 12:30 - Napari
- 12:45 - 13:45 - lunch
- 13:45 - 15:15 - Bio Image Analysis on Notebook
- 15:15 - 15:30 - break
- 15:30 - 17:00 - Bio Image Analysis on Notebook

Schedule day 2:

- 9:30 - 12:30 - Bio Image Analysis on Notebook
- 12:45 - 13:45 - lunch
- 13:45 - 15:15 - Bio Image Analysis on Notebook
- 15:15 - 15:30 - break
- 15:30 - 17:00 - Bio Image Analysis on Notebook

</section>

# Lesson overview

> <i class="fa fa-lock"></i> **License:** [Creative Commons Attribution 4.0 International  License](https://creativecommons.org/licenses/by/4.0/deed.en)
>
> <i class="fa fa-user"></i> **Target Audience:** Researchers, trainers, training providers
>
> <svg xmlns="http://www.w3.org/2000/svg" height="14" width="16" viewBox="0 0 576 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2023 Fonticons, Inc.--><path d="M384 64c0-17.7 14.3-32 32-32H544c17.7 0 32 14.3 32 32s-14.3 32-32 32H448v96c0 17.7-14.3 32-32 32H320v96c0 17.7-14.3 32-32 32H192v96c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32h96V320c0-17.7 14.3-32 32-32h96V192c0-17.7 14.3-32 32-32h96V64z"/></svg> **Level:** Beginner  
>
> <i class="fa fa-arrow-left"></i> **Prerequisites**  
> To be able to follow this course, learners should have knowledge in:
> 
> 1. Understanding of fundamental microscopy concepts
> 2. Access to computational resources (local installation and Google Colab)
> 3. Basic knowledge of Python programming and ability to work with Python environments (understanding of syntax, data structures, data handling, and basic plotting. This can be acquired by completing our [Python introduction e-learning](https://elearning.vib.be/courses/gentle-introduction-to-python/).

>
> <i class="fa fa-bookmark"></i> **Description**  This course consist of .....
> 
> <i class="fa fa-arrow-right"></i> **Learning Outcomes:**  
> By the end of the course, learners will be able to:
>
> 01. Navigate the Napari interface to visualize and interact with multi-dimensional microscopy images.
>
> 02. Import and export image data using Napari and Python libraries (e.g., bioio, NumPy) while preserving metadata.
>
> 03. Apply basic image visualization techniques (e.g., intensity adjustment) within Napari.
>
> 04. Create and manage labels and layers to effectively annotate and organize image data.
>
> 05. Install and use Napari plugins to extend functionality for segmentation and analysis tasks.
>
> 06. Generate simple animations to communicate image analysis results.  
>
> 07. Open and manipulate multi-dimensional microscopy images using Bio.io and Numpy.
>
> 08. Interpret image metadata to understand acquisition parameters and file structure.
>
> 09. Create and validate image files in OME-TIFF format, including metadata for interoperability.
>
> 10. Train and apply deep learning denoising models
>
> 11. Segment microcopy images using both classical approaches and automated tools (e.g., CellPose) to identify biological objects.
>
> 12. Compute and plot quantitative descriptors (e.g., intensity histograms, object counts) for segmented images to support data analysis. 
>
>> Check more about [Bloom's taxonomy](https://cft.vanderbilt.edu/guides-sub-pages/blooms-taxonomy/) to categorize the levels in educational goals
>
> <i class="fa fa-hourglass"></i> **Time estimation**: 12 hours
>
> <i class="fa fa-asterisk"></i> **Requirements:** The (technical) installation requirements are described in the [installations]() section.
>
> <i class="fa fa-envelope-open-text"></i> **Supporting Materials**:
> 
> 1. [Exercises and solutions](link)
> 2. [Slides](link)  
> 
> <i class="fa fa-life-ring"></i> **Acknowledgement**:
>
> * [VIB Technologies](https://www.vib.be/)
> * Benjamin Pavie
> * Nicolas Peredo
> * Tatiana Woller
>
> * [Laboratory of Cell Biology and Histology ](https://www.uantwerpen.be/en/research-groups/celw/)
>
> <i class="fa fa-money-bill"></i> **Funding:**
>
> <i class="fa fa-anchor"></i> **PURL**:  


# Authors and Contributors

Authors

- @[orcid(Benjamin Pavie)](https://orcid.org/0000-0002-0249-3844)

Contributors
- @[orcid(Nicolas Peredo)](https://orcid.org/0000-0002-4670-3700)
- @[orcid(Tim Van De Looverbosch)](https://orcid.org/0000-0002-3065-1395)
- @[orcid(Tatiana Woller)](https://orcid.org/0000-0002-6958-6498)


## Citing this lesson

Please cite as:

  1. ...

# Chapters List

| Chapter | Title                                                   |
| :---- | :------------------------------------------------         |
| 1     | [Napari](link)                                            |
| 2     | [Image IO and Visualization](link)                        |
| 3     | [Imag Processing](link)                                   |
| 4     | [Imag Denoising with N2V](link)                           |
| 5     | [Cell Segmentation with CellPose](link)                   |
| 5     | [Create a Image Analysis Pipeline](link)                   |


# References

Here are some great tips for learning and to get inspired for writing your own pipelines:

- Bioio Documentation([link](https://bioio-devs.github.io/bioio/)) - Library to opne multiple microsocpy file format
- CAREamics Documentation([link](https://careamics.github.io/)) - Library for image restoration deep-learning algorithms
- Cellpose Documentation([link](https://cellpose.readthedocs.io/)) - Anatomical segmentation algorithm
- Scikit-Image Documentation([link](https://scikit-image.org/)) - collection of algorithms for image processing.
- Image.sc Forum ([link](https://forum.image.sc/)) - Active community for bioimage analysis
- BioImage Model Zoo ([link](https://bioimage.io/)) - Pre-trained models and resources
- Napari ([link](https://napari.org/)) - N-dimensional image viewer

# About us

*About VIB and VIB Technologies*

VIB is an entrepreneurial non-profit research institute, with a clear focus on groundbreaking strategic basic research in life sciences and operates in close partnership with the five universities in Flanders – Ghent University, KU Leuven, University of Antwerp, Vrije Universiteit Brussel and Hasselt University.

As part of the VIB Technologies, the 12 VIB Core Facilities, provide support in a wide array of research fields and housing specialized scientific equipment for each discipline. Science and technology go hand in hand. New technologies advance science and often accelerate breakthroughs in scientific research. VIB has a visionary approach to science and technology, founded on its ability to identify and foster new innovations in life sciences.

The goal of VIB Technology Training is to up-skill life scientists to excel in the domains of VIB Technologies, Bioinformatics & AI, Software Development, and Research Data Management.

--------------------------------------------

*Editorial team for this course*

Authors: @[orcid(Benjamin Pavie)](https://orcid.org/0000-0002-0249-3844)

Technical Editors: Benjamin Pavie

License: [![CC BY SA](img/picture003.jpg)](https://creativecommons.org/licenses/by-sa/4.0/deed.en)

```json   @JSONLD
{
  "@context": "https://schema.org/",
  "@type": "LearningResource",
  "@id": "https://elixir-europe-training.github.io/ELIXIR-TrP-TeSS/",
  "http://purl.org/dc/terms/conformsTo": {
    "@type": "CreativeWork",
    "@id": "https://bioschemas.org/profiles/TrainingMaterial/1.0-RELEASE"
  },
  "description": "TeSS, how can I help you? This is our interactive hands-on course about efficient use of the ELIXIR TeSS platform.",
  "keywords": "FAIR, OPEN, Bioinformatics, Teaching, TeSS",
  "name": "TeSS, how can I help you?",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "educationalLevel": "beginner",
  "competencyRequired": "none",
  "teaches": [
    "search events and material in TeSS via direct and faceted search",
    "add manually and automatically events and material to TeSS",
    "extract events and material from TeSS by using TeSS widgets"
  ],
  "audience": "training providers",
  "inLanguage": "en-US",
  "learningResourceType": [
    "tutorial"
  ],
  "author": [
    {
      "@type": "Person",
      "name": "Benjamin Pavie"
    },
  ],
  "contributor": [
    {
      "@type": "Person",
      "name": "Tatiana Woller"
    },
    {
      "@type": "Person",
      "name": "Tim Van De Looverbosch "
    },
    {
      "@type": "Person",
      "name": "Nicolas Peredo"
    }
  ]
}
```











