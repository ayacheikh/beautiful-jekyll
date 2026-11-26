---
layout: page
title: Projects
subtitle: Systems, AI, and machine learning work
share-description: Projects by Aya Cheikh, including a pipelined RISC-V processor, a concurrent search engine in Go, game-playing AI, and machine learning models.
---

<link rel="stylesheet" href="{{ '/assets/css/custom-projects.css' | relative_url }}">

<p class="page-intro">
  A selection of things I've built, from hardware up to machine learning. Code for most of these lives on
  <a href="https://github.com/ayacheikh" target="_blank" rel="noopener">my GitHub</a>.
  For my research and capstone work, see <a href="{{ '/experience' | relative_url }}">Experience</a>.
</p>

<div class="projects-grid">

  <a href="https://github.com/ayacheikh/riscv-pipeline-processor" class="project-item featured" target="_blank" rel="noopener">
    <div class="project-header">
      <h3>5-Stage Pipelined RISC-V Processor</h3>
      <div class="project-meta">Computer Architecture · Apr – May 2026</div>
    </div>
    <div class="project-description">
      Designed and simulated a 64-bit, 5-stage pipelined RISC-V processor with a custom Hazard Unit that resolves
      hazards automatically, with no manual NOPs. It forwards register values from EX/MEM and MEM/WB, detects
      load-use hazards and stalls, and flushes the pipeline on taken branches. Verified against a suite of hazard test programs.
    </div>
    <ul class="chips"><li>RISC-V</li><li>Digital</li><li>Assembly</li><li>Computer architecture</li></ul>
    <div class="project-link">View on GitHub</div>
  </a>

  <a href="https://github.com/ayacheikh/search-engine-" class="project-item featured" target="_blank" rel="noopener">
    <div class="project-header">
      <h3>Concurrent Search Engine</h3>
      <div class="project-meta">Systems Programming · Oct – Nov 2025</div>
    </div>
    <div class="project-description">
      A search engine built from scratch in Go. A multi-stage crawler pipeline (download → extract → clean → index)
      runs on goroutine worker pools connected by channels, respects <code>robots.txt</code> and crawl delays, and
      ranks results with TF-IDF. Storage sits behind a single <code>Index</code> interface with in-memory and SQLite backends.
    </div>
    <ul class="chips"><li>Go</li><li>Goroutines &amp; channels</li><li>SQLite</li><li>TF-IDF</li><li>HTML/CSS</li></ul>
    <div class="project-link">View on GitHub</div>
  </a>

  <a href="https://github.com/ayacheikh/rr-strategy-game" class="project-item featured" target="_blank" rel="noopener">
    <div class="project-header">
      <h3>R-R Strategy Game AI</h3>
      <div class="project-meta">Algorithms &amp; AI · Feb – Mar 2026</div>
    </div>
    <div class="project-description">
      A 16×16 Othello-style strategy game with three AI players: random, heuristic (piece differential plus corner control),
      and minimax with alpha-beta pruning. Simulated 300 games with alternating sides and openings to benchmark
      strategies and evaluate board fairness. The minimax agent won 99% of its games against the random baseline.
    </div>
    <ul class="chips"><li>Python</li><li>Minimax</li><li>Alpha-beta pruning</li><li>Heuristic search</li><li>OOP</li></ul>
    <div class="project-link">View on GitHub</div>
  </a>

  <a href="https://github.com/ayacheikh/course-catalog-chatbot" class="project-item" target="_blank" rel="noopener">
    <div class="project-header">
      <h3>Course Catalog Chatbot</h3>
      <div class="project-meta">Software Development</div>
    </div>
    <div class="project-description">
      An AI-powered chatbot for the University of San Francisco course catalog. Users ask natural-language questions
      about courses (instructors, times, locations, buildings) and get accurate answers grounded in a database.
    </div>
    <ul class="chips"><li>Go</li><li>SQLite</li><li>AI</li><li>Natural language queries</li></ul>
    <div class="project-link">View on GitHub</div>
  </a>

  <a href="https://github.com/ayacheikh/airbnb-price-predictor" class="project-item" target="_blank" rel="noopener">
    <div class="project-header">
      <h3>Airbnb Price Predictor</h3>
      <div class="project-meta">Machine Learning</div>
    </div>
    <div class="project-description">
      A regression model that predicts nightly Airbnb prices from 42K real listings. Covers EDA, imputation, and one-hot
      feature engineering, then compares models on a held-out validation split. A tuned Random Forest reached
      an RMSE of 56.9, versus 98.0 for a linear baseline.
    </div>
    <ul class="chips"><li>Python</li><li>scikit-learn</li><li>pandas</li><li>Random Forest</li><li>Jupyter</li></ul>
    <div class="project-link">View on GitHub</div>
  </a>

  <a href="https://docs.google.com/document/d/1GD4AGBYTycMTabaIfvXTp5-7Z5QzedsbZPzGWokGAqk/edit?usp=sharing" class="project-item" target="_blank" rel="noopener">
    <div class="project-header">
      <h3>Breast Cancer Prediction</h3>
      <div class="project-meta">Machine Learning</div>
    </div>
    <div class="project-description">
      A Random Forest classifier that predicts breast cancer diagnoses from the Wisconsin Breast Cancer dataset.
      Includes a written report on methodology and results.
    </div>
    <ul class="chips"><li>Python</li><li>scikit-learn</li><li>Random Forest</li><li>Classification</li></ul>
    <div class="project-link">View Report</div>
  </a>

</div>
