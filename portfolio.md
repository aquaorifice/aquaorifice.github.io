---
layout: page
title: portfolio
permalink: /portfolio/
---

<style>
.project-card {
    margin-bottom: 40px;
    padding: 30px;
    background: white;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    transition: all 0.3s ease;
}

.project-card:hover {
    box-shadow: 0 8px 16px rgba(0,0,139,0.15);
    transform: translateY(-5px);
}

.project-title {
    font-size: 26px;
    font-weight: bold;
    color: #00008B;
    margin-bottom: 10px;
}

.project-meta {
    color: #666;
    font-style: italic;
    margin-bottom: 15px;
}

.project-description {
    line-height: 1.8;
    color: #333;
    margin-bottom: 15px;
}

.project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 15px;
}

.tag {
    background: #e6f2ff;
    color: #00008B;
    padding: 5px 12px;
    border-radius: 15px;
    font-size: 13px;
    font-weight: 500;
}

.project-links {
    margin-top: 15px;
}

.project-links a {
    margin-right: 15px;
    color: #00008B;
    font-weight: 600;
    text-decoration: none;
}

.project-links a:hover {
    text-decoration: underline;
}
</style>

<p style="font-size: 18px; margin-bottom: 40px; color: #555;">
    Here are some of my key projects from my time at Oracle and during my PhD research.
</p>

## Research Projects

<div class="project-card">
    <div class="project-title">Wavelet Trees for Learned Indexes</div>
    <div class="project-meta">PhD Research | 2024 - 2025</div>
    <div class="project-description">
        <p>
            Exploring wavelet trees as a space-efficient alternative for physical-to-sorted mapping in learned indexes. 
            This work demonstrates the inherent tradeoffs between space and time and how traditional data structures can be evolved to reduce memory footprint while maintaining query performance in modern indexing systems.
        </p>
        <p>
            <strong>Key contributions:</strong> Novel application of wavelet trees to learned indexes, demonstrating significant space savings; and how modifying the structure supports tradeoff between size and performance overhead.
        </p>
        <p>
            This work received an <strong>Honorable Mention Award</strong> at AIDB @ VLDB 2025.
        </p>
    </div>
    <div class="project-tags">
        <span class="tag">Wavelet Trees</span>
        <span class="tag">Learned Indexes</span>
        <span class="tag">Data Structures</span>
        <span class="tag">Space Efficiency</span>
    </div>
    <div class="project-links">
        <a href="#">https://disc.bu.edu/papers/aidb25-saha</a>
        <a href="#">https://github.com/BU-DiSC/wavelet-tree-mapping</a>
    </div>
</div>

<div class="project-card">
    <div class="project-title">AXE: Learned LSM Tuning</div>
    <div class="project-meta">Research Paper | PVLDB (to appear)</div>
    <div class="project-description">
        <p>
            A task decomposition approach to learned LSM tuning that breaks down the complex tuning problem 
            into manageable sub-tasks, improving the efficiency and effectiveness of LSM-tree configuration.
        </p>
    </div>
    <div class="project-tags">
        <span class="tag">LSM Trees</span>
        <span class="tag">Learned Systems</span>
        <span class="tag">Task Decomposition</span>
        <span class="tag">RocksDB</span>
    </div>
    <div class="project-links">
        <a href="#">https://disc.bu.edu/papers/vldb25-huynh</a>
        <a href="#">https://github.com/BU-DiSC/endure</a>
    </div>
</div>

<div class="project-card">
    <div class="project-title">Masters Thesis: Tuning LSM Trees using Bayesian Optimization</div>
    <div class="project-meta">Masters Research | 2022 - 2024</div>
    <div class="project-description">
        <p>
            Developed techniques for automatic tuning of LSM trees using Bayesian optimization, exploring 
            the configuration space to find optimal settings for different workloads.
        </p>
    </div>
    <div class="project-tags">
        <span class="tag">LSM Trees</span>
        <span class="tag">Bayesian Optimization</span>
        <span class="tag">Auto-tuning</span>
    </div>
</div>

---

## Industry Projects

<div class="project-card">
    <div class="project-title">Oracle Communications Session Monitor</div>
    <div class="project-meta">Oracle Corporation | 2019 - 2022</div>
    <div class="project-description">
        <p>
            Built performance tooling, worked on UI migration to OJET, and automation for SIP-centric monitoring, 
            modernizing diagnostics and test coverage for Oracle Communications products.
        </p>
    </div>
    <div class="project-tags">
        <span class="tag">Java</span>
        <span class="tag">TypeScript</span>
        <span class="tag">OJET</span>
        <span class="tag">Automation</span>
        <span class="tag">Testing</span>
    </div>
</div>

---

## Open Source & Side Projects

<div class="project-card">
    <div class="project-title">Kubernetes Talk at KubeCon 2024</div>
    <div class="project-meta">Conference Talk | March 2024</div>
    <div class="project-description">
        <p>
            Presented at KubeCon on [your topic]. This talk covered [key topics covered in your talk].
        </p>
        <p>
            <strong>Watch:</strong> <a href="https://www.youtube.com/watch?v=LEjTcQxxbL8" target="_blank">YouTube Recording</a>
        </p>
    </div>
    <div class="project-tags">
        <span class="tag">Kubernetes</span>
        <span class="tag">Cloud Native</span>
        <span class="tag">Public Speaking</span>
    </div>
</div>

---

<p style="text-align: center; margin-top: 50px; font-size: 16px; color: #666;">
    For more details about any of these projects, feel free to <a href="mailto:anwesha@bu.edu" style="color: #00008B; font-weight: 600;">reach out</a>!
</p>
