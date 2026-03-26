---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# About Me
I am a second-year PhD student at [Huazhong University of Science and Technology (HUST)](https://www.hust.edu.cn/), School of Integrated Circuits. I am supervised by [Prof. Yi Li](https://ismd.hust.edu.cn/info/1077/1257.htm) in [Odysseia Lab](https://www.liyilab.com/).

My research focuses on Computing-in-Memory (CIM) architecture and circuit design, with an emphasis on heterogeneous CIM accelerators for edge LLM and Transformer workloads.

You can download my CV here: [Zhiwei Zhou's Curriculum Vitae](../assets/cv_zhiweizhou.pdf).

If you are interested in my work, please feel free to drop me an email: [zhou_zw@hust.edu.cn](mailto:zhou_zw@hust.edu.cn) | [zw.zhou.2000@gmail.com](mailto:zw.zhou.2000@gmail.com)

{% if site.author.orcid and site.author.orcid != "" %}
ORCID: [{{ site.author.orcid }}]({{ site.author.orcid }})
{% endif %}

Google Scholar: <a href='https://scholar.google.com/citations?user=yu4G0pcAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>

<span class='anchor' id='news'></span>

# News
- *2026.03*: &nbsp;🎉🎉New paper "Outlier-aware FP8 SRAM-CIM macro for edge Transformer" accepted by VLSI 2026!!!
- *2026.02*: &nbsp;🎉🎉New paper "CIM accelerator for Sparse Transformer" accepted by DAC 2026.
- *2026.01*: &nbsp;🎉🎉Our ASP-DAC 2026 paper was selected as a Best Paper Candidate!!
- *2026.01*: &nbsp;🎉🎉New paper "CIM accelerator for Attention-free Transformer" accepted by ISCAS 2026.
- *2025.09*: &nbsp;🎉🎉New paper "Outlier-aware CIM accelerator for Transformer" accepted by ASP-DAC 2026.
- *2024.11*: &nbsp;🎉🎉New paper "Arbitrary-Precision CIM accelerator with Unified INT/FP Arithmetic" accepted by IEEE TCAS-I 2025.

<span class='anchor' id='publications'></span>

# Publications
- [**VLSI'26**] **Zhiwei Zhou†**, Tong Hu†, Jia Chen, Jiancong Li, Yuyang Fu, Yi Li, Xiangshui Miao. **A 40nm 24.85-to-80.59 TFLOPS/W FP8 Computing-in-Memory Macro with Outlier-Aware Hierarchical-Alignment for Edge Transformers** (Co-first Author).
- [**DAC'26**] Tong Li†, **Zhiwei Zhou†**, Jiancong Li, Yuyang Fu, Yingjie Yu, Tong Hu, Jia Chen, Yi Li, Xiangshui Miao. **HP-CIM: A Computing-in-Memory Transformer Accelerator with ReRAM-based Hash Predictor for Attention Sparsity Exploitation** (Co-first Author).
- [**ISCAS'26**] **Zhiwei Zhou**, Yuyang Fu, Jiancong Li, Yi Li, Xiangshui Miao. **Energy-Efficient Acceleration of Fourier-Based Transformers on RRAM-CIM via Mixed-Precision and DFT Symmetry**.
- [**ASP-DAC'26**] **Zhiwei Zhou**, Tong Hu, Han Bao, Houji Zhou, Yuyang Fu, Jiancong Li, Jia Chen, Yi Li, Xiangshui Miao. [**OAH-CIM: Outlier-Aware Hybrid RRAM-SRAM CIM Accelerator with Variation-Robust Sparsity**](https://ieeexplore.ieee.org/document/11420538) (Best Paper Candidate).
- [**TCAS-I'25**] **Zhiwei Zhou†**, Jiancong Li†, Han Jia†, Ling Yang, Houji Zhou, Han Bao, Yuyang Fu, Yi Li, Xiangshui Miao. [**ArPCIM: An Arbitrary-Precision Analog Computing-in-Memory Accelerator With Unified INT/FP Arithmetic**](https://ieeexplore.ieee.org/document/10752350).

<span class='anchor' id='education'></span>

# Education
- *2024.09 - Present*, PhD in Integrated Circuit Science and Engineering, Huazhong University of Science and Technology, Wuhan, China.
- *2022.09 - 2024.09*, MS in Integrated Circuit Science and Engineering, Huazhong University of Science and Technology, Wuhan, China.
- *2018.09 - 2022.06*, BS in Electronic Science and Technology, Huazhong University of Science and Technology, Wuhan, China.

<span class='anchor' id='honors-and-awards'></span>

# Honors and Awards
- *2025.08*: The 8th China Postgraduate IC Innovation Competition, National Second Prize (Captain).
- *2024.08*: The 7th China Postgraduate IC Innovation Competition, National First Prize (Member).
- *2023.10*: The 20th China Postgraduate Mathematical Contest in Modeling, National Third Prize (Captain).
- *2023.08*: The 6th China Postgraduate IC Innovation Competition, National Second Prize (Member).
- *2022.06*: Outstanding Graduate, Huazhong University of Science and Technology.

<span class='anchor' id='patents-and-software'></span>

# Patents and Software
## Patents
1. **Yi Li, Zhiwei Zhou**, *A Universal In-Memory Matrix-Tensor Processor and Its Operation Method*, Application No. 2023105941388.
2. **Yi Li, Zhiwei Zhou**, *A Joint Software-Hardware Simulation and Optimization System for Memristive Computing-in-Memory*, Application No. 2025110431717.
3. **Yi Li, Zhiwei Zhou**, *A Universal Computing-in-Memory Simulation Method and System*, Application No. 2025110431736.

## Software Copyright
1. **Yi Li, Zhiwei Zhou**, *Universal Memristive Computing-in-Memory Simulator Software V1.0*, Registration No. 2025SR1838416.

<span class='anchor' id='technical-skills'></span>

# Technical Skills
- **EDA Tools**: Cadence (Virtuoso, Innovus), Synopsys (Design Compiler, PrimeTime), CACTI 7.0.
- **Programming**: Verilog HDL, Python (PyTorch), C/C++.
- **Frameworks**: Developer of [MemIntelli](https://github.com/HUST-ISMD-Odyssey/MemIntelli).

<span class='anchor' id='visitor-analytics'></span>

# Visitor Analytics
{% if site.busuanzi_enabled %}
- Visitors: <span id="busuanzi_value_site_uv">--</span>
- Page views: <span id="busuanzi_value_site_pv">--</span>
<script async src="//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>
{% endif %}

{% if site.clustrmaps_id and site.clustrmaps_id != "" %}
<script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d={{ site.clustrmaps_id }}&cl=ffffff&w=a"></script>
{% else %}
Set `clustrmaps_id` in `_config.yml` after registering your site on [ClustrMaps](https://clustrmaps.com) to show the visitor world map.
{% endif %}
