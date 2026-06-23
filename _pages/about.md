---
permalink: /
title: ""
excerpt: ""
author_profile: false
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

<section class="profile-hero" id="about-me">
  <div class="profile-hero__inner">
    <img class="profile-mark" src="{{ '/images/android-chrome-192x192.png' | relative_url }}" alt="Zhiwei Zhou logo">
    <div>
      <p class="eyebrow">Computing-in-Memory Architecture and Circuit Design</p>
      <h1>Zhiwei Zhou</h1>
      <p class="profile-subtitle">PhD student, School of Integrated Circuits, Huazhong University of Science and Technology</p>
      <p>
        I am a PhD student at <a href="https://www.hust.edu.cn/" target="_blank" rel="noopener">Huazhong University of Science and Technology (HUST)</a>, supervised by <a href="https://ismd.hust.edu.cn/info/1077/1257.htm" target="_blank" rel="noopener">Prof. Yi Li</a> in <a href="https://www.liyilab.com/" target="_blank" rel="noopener">Odysseia Lab</a>. My research focuses on compute-in-memory (CIM) architecture and circuit design, especially heterogeneous CIM accelerators for edge LLM and Transformer workloads.
      </p>
      <div class="profile-links" aria-label="Profile links">
        <a href="mailto:zhou_zw@hust.edu.cn"><i class="fas fa-envelope" aria-hidden="true"></i>Email</a>
        <a href="https://scholar.google.com/citations?user=yu4G0pcAAAAJ" target="_blank" rel="noopener"><i class="fas fa-graduation-cap" aria-hidden="true"></i>Google Scholar</a>
        <a href="https://github.com/zhuizhou" target="_blank" rel="noopener"><i class="fab fa-github" aria-hidden="true"></i>GitHub</a>
        <a href="{{ '/assets/cv_zhiweizhou.pdf' | relative_url }}" target="_blank" rel="noopener"><i class="fas fa-file-pdf" aria-hidden="true"></i>CV</a>
      </div>
      <p class="scholar-badge">
        <a href="https://scholar.google.com/citations?user=yu4G0pcAAAAJ" target="_blank" rel="noopener">
          <img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations" alt="Google Scholar citations">
        </a>
      </p>
    </div>
  </div>
</section>

<section class="site-section" id="research">
  <h2>Research Interests</h2>
  <div class="research-list">
    <article>
      <h3>Compute-in-Memory Accelerators</h3>
      <p>Architectures and circuits that move matrix and tensor operations closer to memory for efficient AI workloads.</p>
    </article>
    <article>
      <h3>Transformer and Edge LLM Hardware</h3>
      <p>Mixed-precision, sparsity-aware, and outlier-aware acceleration for Transformer inference under tight energy budgets.</p>
    </article>
    <article>
      <h3>Digital and Analog CIM Co-design</h3>
      <p>Cross-layer design spanning device non-idealities, SRAM/ReRAM macros, arithmetic formats, and compiler-friendly dataflows.</p>
    </article>
  </div>
</section>

<section class="site-section" id="news">
  <h2>News</h2>
  <ul class="timeline-list">
    <li><time>2026.03</time><span>Paper accepted by VLSI 2026: "A 40nm 24.85-to-80.59 TFLOPS/W FP8 Computing-in-Memory Macro with Outlier-Aware Hierarchical-Alignment for Edge Transformers."</span></li>
    <li><time>2026.02</time><span>Paper accepted by DAC 2026: "HP-CIM: A Computing-in-Memory Transformer Accelerator with ReRAM-based Hash Predictor for Attention Sparsity Exploitation."</span></li>
    <li><time>2026.01</time><span>ASP-DAC 2026 paper selected as a Best Paper Candidate.</span></li>
    <li><time>2026.01</time><span>Paper accepted by ISCAS 2026: "Energy-Efficient Acceleration of Fourier-Based Transformers on RRAM-CIM via Mixed-Precision and DFT Symmetry."</span></li>
    <li><time>2025.09</time><span>Paper accepted by ASP-DAC 2026: "OAH-CIM: Outlier-Aware Hybrid RRAM-SRAM CIM Accelerator with Variation-Robust Sparsity."</span></li>
    <li><time>2024.11</time><span>Paper accepted by IEEE TCAS-I: "ArPCIM: An Arbitrary-Precision Analog Computing-in-Memory Accelerator With Unified INT/FP Arithmetic."</span></li>
  </ul>
</section>

<section class="site-section" id="publications">
  <h2>Selected Publications</h2>
  <ol class="publication-list">
    <li class="publication-item">
      <div class="publication-venue">VLSI<br>2026</div>
      <article>
        <h3>A 40nm 24.85-to-80.59 TFLOPS/W FP8 Computing-in-Memory Macro with Outlier-Aware Hierarchical-Alignment for Edge Transformers</h3>
        <p class="publication-authors"><strong>Zhiwei Zhou</strong><sup>*</sup>, Tong Hu<sup>*</sup>, Jia Chen, Jiancong Li, Yuyang Fu, Yi Li, Xiangshui Miao</p>
        <p class="publication-meta">2026 IEEE Symposium on VLSI Technology and Circuits. <span class="note">* Equal contribution.</span></p>
        <details class="abstract-toggle">
          <summary>Abs</summary>
          <p>This paper presents a digital compute-in-memory (CIM)-based macro tailored for edge Transformer acceleration. It has three features: 1) a Hierarchical Dual-Exponent Alignment scheme that separates outliers from normal values, achieving near-ideal accuracy with minimal overhead; 2) a Sign-Magnitude Input Serial Pipelined Aligner (SMSPA) that reduces area and power by 41.1% and 34.1%; and 3) a Shift-Concat based Sign-Inverse Adder Tree (SSAT) that saves accumulation area and power by 25.9% and 18.2%. The macro achieves 24.85-80.59 TFLOPS/W in FP8. Measurements demonstrate up to 6.66x improvement in energy efficiency compared with state-of-the-art post-alignment FP-CIM schemes while maintaining high accuracy across tasks.</p>
        </details>
      </article>
    </li>
    <li class="publication-item">
      <div class="publication-venue">DAC<br>2026</div>
      <article>
        <h3>HP-CIM: A Computing-in-Memory Transformer Accelerator with ReRAM-based Hash Predictor for Attention Sparsity Exploitation</h3>
        <p class="publication-authors">Tong Li<sup>*</sup>, <strong>Zhiwei Zhou</strong><sup>*</sup>, Jiancong Li, Yuyang Fu, Yingjie Yu, Tong Hu, Jia Chen, Yi Li, Xiangshui Miao</p>
        <p class="publication-meta">Design Automation Conference (DAC), 2026. <span class="note">* Equal contribution.</span></p>
        <details class="abstract-toggle">
          <summary>Abs</summary>
          <p>Transformer models have become the cornerstone of modern artificial intelligence, but attention operations and large-scale matrix multiplications incur high latency and energy consumption. Hybrid CIM architectures that integrate ReRAM and SRAM are promising for Transformer acceleration, yet self-attention sparsity creates redundant computation. HP-CIM employs a ReRAM-based hash predictor (ReHP) to leverage attention sparsity efficiently. ReHP uses intrinsic ReRAM conductance variation for low-cost hash projection and integrates a ReRAM content-addressable memory with a K-winner-take-all circuit for highly parallel, energy-efficient Top-K matching. An optimizable bias-filling strategy restores model accuracy with a learnable bias that compensates for information loss during hash prediction. Across multiple Transformer models and tasks, HP-CIM achieves 9.05-310.04x higher energy efficiency and 2.48-16.93x speedup over state-of-the-art CIM-based Transformer accelerators.</p>
        </details>
      </article>
    </li>
    <li class="publication-item">
      <div class="publication-venue">ISCAS<br>2026</div>
      <article>
        <h3>Energy-Efficient Acceleration of Fourier-Based Transformers on RRAM-CIM via Mixed-Precision and DFT Symmetry</h3>
        <p class="publication-authors"><strong>Zhiwei Zhou</strong>, Yuyang Fu, Jiancong Li, Yi Li, Xiangshui Miao</p>
        <p class="publication-meta">IEEE International Symposium on Circuits and Systems (ISCAS), 2026.</p>
      </article>
    </li>
    <li class="publication-item">
      <div class="publication-venue">ASP-DAC<br>2026</div>
      <article>
        <h3>OAH-CIM: Outlier-Aware Hybrid RRAM-SRAM CIM Accelerator with Variation-Robust Sparsity</h3>
        <p class="publication-authors"><strong>Zhiwei Zhou</strong>, Tong Hu, Han Bao, Houji Zhou, Yuyang Fu, Jiancong Li, Jia Chen, Yi Li, Xiangshui Miao</p>
        <p class="publication-meta">Asia and South Pacific Design Automation Conference (ASP-DAC), 2026. <span class="note">Best Paper Candidate.</span></p>
        <p class="publication-links"><a href="https://ieeexplore.ieee.org/document/11420538" target="_blank" rel="noopener">HTML</a></p>
      </article>
    </li>
    <li class="publication-item">
      <div class="publication-venue">TCAS-I<br>2025</div>
      <article>
        <h3>ArPCIM: An Arbitrary-Precision Analog Computing-in-Memory Accelerator With Unified INT/FP Arithmetic</h3>
        <p class="publication-authors"><strong>Zhiwei Zhou</strong><sup>*</sup>, Jiancong Li<sup>*</sup>, Han Jia<sup>*</sup>, Ling Yang, Houji Zhou, Han Bao, Yuyang Fu, Yi Li, Xiangshui Miao</p>
        <p class="publication-meta">IEEE Transactions on Circuits and Systems I: Regular Papers, 2025. <span class="note">* Equal contribution.</span></p>
        <p class="publication-links"><a href="https://ieeexplore.ieee.org/document/10752350" target="_blank" rel="noopener">HTML</a></p>
      </article>
    </li>
  </ol>
</section>

<section class="site-section" id="education">
  <h2>Education</h2>
  <ul class="timeline-list compact">
    <li><time>2024.09 - Present</time><span>PhD in Integrated Circuit Science and Engineering, Huazhong University of Science and Technology, Wuhan, China.</span></li>
    <li><time>2022.09 - 2024.09</time><span>MS in Integrated Circuit Science and Engineering, Huazhong University of Science and Technology, Wuhan, China.</span></li>
    <li><time>2018.09 - 2022.06</time><span>BS in Electronic Science and Technology, Huazhong University of Science and Technology, Wuhan, China.</span></li>
  </ul>
</section>

<section class="site-section" id="honors-and-awards">
  <h2>Honors and Awards</h2>
  <ul class="timeline-list compact">
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
      <h3>Technical Skills</h3>
      <p><strong>EDA:</strong> Cadence Virtuoso, Innovus, Synopsys Design Compiler, PrimeTime, CACTI 7.0.</p>
      <p><strong>Programming:</strong> Verilog HDL, Python/PyTorch, C/C++.</p>
      <p><strong>Frameworks:</strong> Developer of <a href="https://github.com/HUST-ISMD-Odyssey/MemIntelli" target="_blank" rel="noopener">MemIntelli</a>.</p>
    </article>
  </div>
</section>

<section class="site-section visitor-panel" id="visitor-analytics">
  <h2>Visitor Analytics</h2>
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
  {% else %}
  <p class="note">Set <code>clustrmaps_id</code> in <code>_config.yml</code> to show the visitor world map.</p>
  {% endif %}
</section>
