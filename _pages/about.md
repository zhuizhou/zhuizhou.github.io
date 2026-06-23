---
permalink: /
title: ""
excerpt: ""
author_profile: false
sidebar:
  - title: "About"
    text: |
      <nav class="about-toc" aria-label="About page sections">
        <a href="#research-interests">Research Interests</a>
        <a href="#news">News</a>
        <a href="#selected-publications">Selected Publications</a>
        <a href="#education">Education</a>
        <a href="#research-experience">Research Experience</a>
        <a href="#honors-and-awards">Honors and Awards</a>
        <a href="#patents-and-software">Patents and Software</a>
        <a href="#technical-skills">Technical Skills</a>
        <a href="#visitor">Visitor</a>
      </nav>
redirect_from:
  - /about/
  - /about.html
---

{% assign selected_publications = site.data.publications | where: "selected", true %}
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@main/" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/main/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<section class="profile-hero" id="about">
  <div class="profile-hero__inner">
    <img class="profile-mark" src="{{ '/images/profile.jpg' | relative_url }}" alt="Zhiwei Zhou">
    <div>
      <h1>Zhiwei Zhou</h1>
      <p class="profile-subtitle">PhD student, School of Integrated Circuits, Huazhong University of Science and Technology</p>
      <p>
        I am a PhD student at <a href="https://www.hust.edu.cn/" target="_blank" rel="noopener">Huazhong University of Science and Technology (HUST)</a>, supervised by <a href="https://ismd.hust.edu.cn/info/1077/1257.htm" target="_blank" rel="noopener">Prof. Yi Li</a> in <a href="https://www.liyilab.com/" target="_blank" rel="noopener">Odysseia Lab</a>. My research focuses on compute-in-memory (CIM) architecture and circuit design for efficient AI acceleration.
      </p>
      <div class="profile-links" aria-label="Profile links">
        <a href="mailto:zhou_zw@hust.edu.cn"><i class="fas fa-envelope" aria-hidden="true"></i>Email</a>
        <a href="https://scholar.google.com/citations?user=yu4G0pcAAAAJ" target="_blank" rel="noopener"><i class="fas fa-graduation-cap" aria-hidden="true"></i>Google Scholar</a>
        <a href="https://github.com/zhuizhou" target="_blank" rel="noopener"><i class="fab fa-github" aria-hidden="true"></i>GitHub</a>
        <a href="{{ '/assets/cv_zhiweizhou.pdf' | relative_url }}" target="_blank" rel="noopener"><i class="fas fa-file-pdf" aria-hidden="true"></i>CV</a>
      </div>
      <div class="scholar-summary">
        <a href="https://scholar.google.com/citations?user=yu4G0pcAAAAJ" target="_blank" rel="noopener">Google Scholar: Cited by {{ site.google_scholar_citations }}</a>
        <img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations" alt="Google Scholar citations">
      </div>
    </div>
  </div>
</section>

<section class="site-section" id="research-interests">
  <h2>Research Interests</h2>
  <div class="research-list">
    <article>
      <h3>Compute-in-Memory Accelerators</h3>
      <p>Architecture and circuit co-design for efficient matrix, tensor, and Transformer workloads near memory.</p>
    </article>
    <article>
      <h3>Transformer and Edge LLM Hardware</h3>
      <p>Mixed-precision, sparsity-aware, and outlier-aware acceleration under tight energy and area budgets.</p>
    </article>
    <article>
      <h3>RRAM/SRAM CIM Systems</h3>
      <p>Cross-layer design spanning devices, macros, arithmetic formats, dataflows, and simulation frameworks.</p>
    </article>
  </div>
</section>

<section class="site-section" id="news">
  <h2>News</h2>
  <ul class="timeline-list">
    <li><time>2026.05</time><span>Started a postgraduate visiting appointment at HKUST ECE with Prof. Fengbin Tu.</span></li>
    <li><time>2026.03</time><span>Paper accepted by VLSI 2026: "A 40nm 24.85-to-80.59 TFLOPS/W FP8 Computing-in-Memory Macro with Outlier-Aware Hierarchical-Alignment for Edge Transformers."</span></li>
    <li><time>2026.02</time><span>Paper accepted by DAC 2026: "HP-CIM: A Computing-in-Memory Transformer Accelerator with ReRAM-based Hash Predictor for Attention Sparsity Exploitation."</span></li>
    <li><time>2026.01</time><span>ASP-DAC 2026 paper selected as a Best Paper Candidate.</span></li>
    <li><time>2026.01</time><span>Paper accepted by ISCAS 2026: "Energy-Efficient Acceleration of Fourier-Based Transformers on RRAM-CIM via Mixed-Precision and DFT Symmetry."</span></li>
    <li><time>2024.11</time><span>Paper accepted by IEEE TCAS-I: "ArPCIM: An Arbitrary-Precision Analog Computing-in-Memory Accelerator With Unified INT/FP Arithmetic."</span></li>
  </ul>
</section>

<section class="site-section" id="selected-publications">
  <h2>Selected Publications</h2>
  {% include publication-list.html publications=selected_publications %}
  <p class="section-more"><a href="{{ '/publications/' | relative_url }}">Full publication list</a></p>
</section>

<section class="site-section" id="education">
  <h2>Education</h2>
  <ul class="timeline-list compact">
    <li><time>2024.09 - Present</time><span>PhD in Integrated Circuit Science and Engineering, Huazhong University of Science and Technology, Wuhan, China.</span></li>
    <li><time>2022.09 - 2024.09</time><span>MS in Integrated Circuit Science and Engineering, Huazhong University of Science and Technology, Wuhan, China.</span></li>
    <li><time>2018.09 - 2022.06</time><span>BS in Electronic Science and Technology, Huazhong University of Science and Technology, Wuhan, China.</span></li>
  </ul>
</section>

<section class="site-section" id="research-experience">
  <h2>Research Experience</h2>
  <ul class="timeline-list compact">
    <li><time>2026.05 - 2026.11</time><span>Postgraduate visiting student, Department of Electronic and Computer Engineering, The Hong Kong University of Science and Technology, with Prof. Fengbin Tu.</span></li>
  </ul>
</section>

<section class="site-section" id="honors-and-awards">
  <h2>Honors and Awards</h2>
  <ul class="timeline-list compact">
    <li><time>2026.01</time><span>ASP-DAC 2026 Best Paper Candidate.</span></li>
    <li><time>2025.08</time><span>The 8th China Postgraduate IC Innovation Competition, National Second Prize (Captain).</span></li>
    <li><time>2024.08</time><span>The 7th China Postgraduate IC Innovation Competition, National First Prize (Member).</span></li>
    <li><time>2023.10</time><span>The 20th China Postgraduate Mathematical Contest in Modeling, National Third Prize (Captain).</span></li>
    <li><time>2023.08</time><span>The 6th China Postgraduate IC Innovation Competition, National Second Prize (Member).</span></li>
    <li><time>2022.06</time><span>Outstanding Graduate, Huazhong University of Science and Technology.</span></li>
  </ul>
</section>

<section class="site-section" id="patents-and-software">
  <h2>Patents and Software</h2>
  <div class="two-column-list">
    <article>
      <h3>Patents</h3>
      <ol>
        <li><strong>Yi Li, Zhiwei Zhou</strong>, A Universal In-Memory Matrix-Tensor Processor and Its Operation Method, Application No. 2023105941388.</li>
        <li><strong>Yi Li, Zhiwei Zhou</strong>, A Joint Software-Hardware Simulation and Optimization System for Memristive Computing-in-Memory, Application No. 2025110431717.</li>
        <li><strong>Yi Li, Zhiwei Zhou</strong>, A Universal Computing-in-Memory Simulation Method and System, Application No. 2025110431736.</li>
      </ol>
    </article>
    <article>
      <h3>Software</h3>
      <ol>
        <li><strong>Yi Li, Zhiwei Zhou</strong>, Universal Memristive Computing-in-Memory Simulator Software V1.0, Registration No. 2025SR1838416.</li>
      </ol>
    </article>
  </div>
</section>

<section class="site-section" id="technical-skills">
  <h2>Technical Skills</h2>
  <div class="skill-grid">
    <p><strong>EDA:</strong> Cadence Virtuoso, Innovus, Synopsys Design Compiler, PrimeTime, CACTI 7.0.</p>
    <p><strong>Programming:</strong> Verilog HDL, Python/PyTorch, C/C++.</p>
    <p><strong>Research Tools:</strong> CIM modeling, circuit simulation, architecture exploration, Transformer acceleration.</p>
    <p><strong>Open Source:</strong> Developer of <a href="https://github.com/HUST-ISMD-Odyssey/MemIntelli" target="_blank" rel="noopener">MemIntelli</a>.</p>
  </div>
</section>

<section class="site-section visitor-panel" id="visitor">
  <h2>Visitor</h2>
  {% if site.busuanzi_enabled %}
  <div class="visitor-stats" aria-label="Visitor counters">
    <span><strong id="busuanzi_value_site_uv">--</strong> visitors</span>
    <span><strong id="busuanzi_value_site_pv">--</strong> page views</span>
  </div>
  <script async src="https://busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>
  {% endif %}

  {% if site.clustrmaps_id and site.clustrmaps_id != "" %}
  <div class="visitor-map">
    <script type="text/javascript" id="clustrmaps" src="https://clustrmaps.com/map_v2.js?d={{ site.clustrmaps_id }}&cl=ffffff&w=a"></script>
  </div>
  {% endif %}
</section>
