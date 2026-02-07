---
layout: default
title: Home
---

<style>
/* ===== Global ===== */
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
  line-height: 1.7;
}

/* ===== Profile Header ===== */
.profile-header {
  display: flex;
  align-items: flex-start;
  gap: 30px;
  margin-bottom: 30px;
  padding: 30px;
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  border-radius: 12px;
  border-left: 4px solid #2c5f2d;
}

.profile-info h1 {
  margin: 0 0 8px 0;
  font-size: 2em;
  color: #1a1a2e;
}

.profile-info .subtitle {
  font-size: 1.1em;
  color: #555;
  margin-bottom: 12px;
}

.profile-info .affiliation {
  color: #2c5f2d;
  font-weight: 600;
}

.profile-links {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 15px;
}

.profile-links a {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 6px 14px;
  background: #fff;
  border: 1px solid #ddd;
  border-radius: 20px;
  color: #333;
  text-decoration: none;
  font-size: 0.9em;
  transition: all 0.2s;
}

.profile-links a:hover {
  background: #2c5f2d;
  color: #fff;
  border-color: #2c5f2d;
}

/* ===== Section Styles ===== */
.section {
  margin-bottom: 35px;
}

.section h2 {
  color: #1a1a2e;
  border-bottom: 2px solid #2c5f2d;
  padding-bottom: 8px;
  margin-bottom: 20px;
  font-size: 1.5em;
}

/* ===== News ===== */
.news-list {
  list-style: none;
  padding: 0;
}

.news-list li {
  padding: 8px 0;
  border-bottom: 1px dashed #eee;
  display: flex;
  gap: 12px;
}

.news-date {
  color: #888;
  font-size: 0.9em;
  min-width: 90px;
  font-family: monospace;
}

.news-badge {
  display: inline-block;
  padding: 1px 8px;
  border-radius: 4px;
  font-size: 0.8em;
  font-weight: 600;
  color: #fff;
}

.badge-new { background: #e74c3c; }
.badge-pub { background: #3498db; }

/* ===== Research Interests ===== */
.research-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.research-tag {
  display: inline-block;
  padding: 8px 18px;
  background: #f0f7f0;
  border: 1px solid #2c5f2d;
  border-radius: 25px;
  color: #2c5f2d;
  font-weight: 500;
  font-size: 0.95em;
}

/* ===== Publications ===== */
.pub-item {
  padding: 16px 20px;
  margin-bottom: 15px;
  background: #fafafa;
  border-left: 3px solid #2c5f2d;
  border-radius: 0 8px 8px 0;
  transition: box-shadow 0.2s;
}

.pub-item:hover {
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
}

.pub-title {
  font-weight: 700;
  color: #1a1a2e;
  font-size: 1.05em;
  margin-bottom: 4px;
}

.pub-authors {
  color: #555;
  font-size: 0.93em;
  margin-bottom: 4px;
}

.pub-authors .me {
  color: #2c5f2d;
  font-weight: 700;
  text-decoration: underline;
}

.pub-venue {
  font-style: italic;
  color: #777;
  font-size: 0.92em;
}

.pub-venue .venue-badge {
  display: inline-block;
  padding: 1px 8px;
  background: #2c5f2d;
  color: #fff;
  border-radius: 4px;
  font-style: normal;
  font-size: 0.85em;
  font-weight: 600;
  margin-right: 6px;
}

.pub-year-header {
  font-size: 1.2em;
  font-weight: 700;
  color: #2c5f2d;
  margin: 20px 0 10px 0;
  display: flex;
  align-items: center;
  gap: 8px;
}

/* ===== Education ===== */
.edu-item {
  display: flex;
  gap: 15px;
  padding: 12px 0;
  border-bottom: 1px solid #f0f0f0;
}

.edu-year {
  min-width: 110px;
  color: #888;
  font-family: monospace;
  font-size: 0.95em;
  padding-top: 2px;
}

.edu-detail h4 {
  margin: 0 0 3px 0;
  color: #1a1a2e;
}

.edu-detail p {
  margin: 0;
  color: #666;
  font-size: 0.93em;
}

/* ===== Experience ===== */
.exp-item {
  display: flex;
  gap: 15px;
  padding: 12px 0;
  border-bottom: 1px solid #f0f0f0;
}

.exp-year {
  min-width: 110px;
  color: #888;
  font-family: monospace;
  font-size: 0.95em;
  padding-top: 2px;
}

.exp-detail h4 {
  margin: 0 0 3px 0;
  color: #1a1a2e;
}

.exp-detail p {
  margin: 0;
  color: #666;
  font-size: 0.93em;
}

/* ===== Footer ===== */
.contact-section {
  background: #f8f9fa;
  padding: 20px 25px;
  border-radius: 8px;
  text-align: center;
}

.contact-section a {
  color: #2c5f2d;
  font-weight: 600;
}

/* ===== Responsive ===== */
@media (max-width: 600px) {
  .profile-header {
    flex-direction: column;
    padding: 20px;
  }
  .edu-item, .exp-item {
    flex-direction: column;
    gap: 5px;
  }
  .news-list li {
    flex-direction: column;
    gap: 4px;
  }
}
</style>

<!-- ==================== PROFILE HEADER ==================== -->
<div class="profile-header">
  <div class="profile-info">
    <h1>Yunhe Pang <span style="font-size:0.6em; color:#666;">（庞运河）</span></h1>
    <div class="subtitle">
      Ph.D. Candidate in Computer Science and Technology<br>
      <span class="affiliation">Sun Yat-sen University (SYSU) 🏫</span>
    </div>
    <div class="profile-links">
      <a href="mailto:pangyh8@mail2.sysu.edu.cn">📧 Email</a>
      <a href="https://scholar.google.com/citations?user=doF4h50AAAAJ&hl=zh-CN&oi=ao" target="_blank">🎓 Google Scholar</a>
      <a href="https://github.com/pangaass" target="_blank">💻 GitHub</a>
      <a href="https://dblp.org/search#q=Yunhe%20Pang" target="_blank">📚 DBLP</a>
      <a href="https://www.semanticscholar.org/search?q=Yunhe+Pang&sort=relevance" target="_blank">📖 Semantic Scholar</a>
    </div>
  </div>
</div>

<!-- ==================== ABOUT ME ==================== -->
<div class="section">
<h2>🧑‍🔬 About Me</h2>

<p>
I am a first-year Ph.D. student at <strong>Sun Yat-sen University (SYSU)</strong>, advised by Prof. <a href="https://scholar.google.com/citations?user=PLACEHOLDER" target="_blank">Yanghui Rao</a>. My research focuses on <strong>Large Language Models (LLMs)</strong> and <strong>Data Mining</strong>, with applications in academic knowledge graphs, sentiment analysis, and anomaly detection.
</p>

<p>
Currently, I am interning at <strong><a href="https://www.zhipuai.cn/" target="_blank">Zhipu AI</a></strong>, working on cutting-edge AI technologies related to large language models.
</p>

<p>
Before joining SYSU, I earned my Master's degree (2020–2023) and Bachelor's degree (2016–2020) in <strong>Computer Science and Technology</strong> from <strong>North China Electric Power University (NCEPU)</strong>.
</p>

</div>

<!-- ==================== NEWS ==================== -->
<div class="section">
<h2>🔥 News</h2>

<ul class="news-list">
  <li>
    <span class="news-date">2025.05</span>
    <span><span class="news-badge badge-new">New</span> One paper accepted by <strong>KDD 2025</strong> — GuARD for anomaly detection!</span>
  </li>
  <li>
    <span class="news-date">2025.05</span>
    <span><span class="news-badge badge-new">New</span> One paper accepted by <strong>ACL 2025</strong> — CoE for emotion recognition!</span>
  </li>
  <li>
    <span class="news-date">2024.05</span>
    <span><span class="news-badge badge-pub">Pub</span> One paper accepted by <strong>KDD 2024</strong> — OAG-Bench benchmark!</span>
  </li>
  <li>
    <span class="news-date">2024.09</span>
    <span>Started Ph.D. journey at <strong>Sun Yat-sen University</strong>.</span>
  </li>
  <li>
    <span class="news-date">2023.07</span>
    <span>Joined <strong>Zhipu AI</strong> as a Research Intern.</span>
  </li>
</ul>

</div>

<!-- ==================== RESEARCH INTERESTS ==================== -->
<div class="section">
<h2>🔬 Research Interests</h2>

<div class="research-tags">
  <span class="research-tag">Large Language Models (LLMs)</span>
  <span class="research-tag">Data Mining</span>
  <span class="research-tag">Academic Knowledge Graphs</span>
  <span class="research-tag">Anomaly Detection</span>
  <span class="research-tag">Sentiment Analysis</span>
  <span class="research-tag">Graph Neural Networks</span>
</div>

</div>

<!-- ==================== PUBLICATIONS ==================== -->
<div class="section">
<h2>📝 Selected Publications</h2>

<p style="color:#888; font-size:0.9em;">
  (* denotes equal contribution, <strong><u>bold & underlined</u></strong> denotes me)
  <br>
  Full list on <a href="https://scholar.google.com/citations?user=doF4h50AAAAJ&hl=zh-CN&oi=ao" target="_blank">Google Scholar</a>.
</p>

<div class="pub-year-header">📅 2025</div>

<div class="pub-item">
  <div class="pub-title">GuARD: Effective Anomaly Detection through a Text-Rich and Graph-Informed Language Model</div>
  <div class="pub-authors"><span class="me">Yunhe Pang</span>, Bo Chen, Fanjin Zhang, Yanghui Rao, Evgeny Kharlamov, Jie Tang</div>
  <div class="pub-venue"><span class="venue-badge">KDD 2025</span> ACM SIGKDD Conference on Knowledge Discovery and Data Mining</div>
</div>

<div class="pub-item">
  <div class="pub-title">CoE: A Clue of Emotion Framework for Emotion Recognition in Conversations</div>
  <div class="pub-authors">Zhiyu Shen, <span class="me">Yunhe Pang</span>, Yanghui Rao, Jianxing Yu</div>
  <div class="pub-venue"><span class="venue-badge">ACL 2025</span> Annual Meeting of the Association for Computational Linguistics</div>
</div>

<div class="pub-year-header">📅 2024</div>

<div class="pub-item">
  <div class="pub-title">OAG-Bench: A Human-Curated Benchmark for Academic Graph Mining</div>
  <div class="pub-authors">Fanjin Zhang, Shijie Shi, Yifan Zhu, Bo Chen, Yukuo Cen, Jifan Yu, Yelin Chen, Lulu Wang, Qingfei Zhao, Yuqing Cheng, Tianyi Han, Yuwei An, Dan Zhang, Weng Lam Tam, Kun Cao, <span class="me">Yunhe Pang</span>, Xinyu Guan, Huihui Yuan, Jian Song, Xiaoyan Li, Yuxiao Dong, Jie Tang</div>
  <div class="pub-venue"><span class="venue-badge">KDD 2024</span> ACM SIGKDD Conference on Knowledge Discovery and Data Mining</div>
</div>

<div class="pub-year-header">📅 2022</div>

<div class="pub-item">
  <div class="pub-title">Learnable Dependency-based Double Graph Structure for Aspect-based Sentiment Analysis</div>
  <div class="pub-authors">Yinglong Ma, <span class="me">Yunhe Pang</span></div>
  <div class="pub-venue"><span class="venue-badge">COLING 2022</span> International Conference on Computational Linguistics</div>
</div>

</div>

<!-- ==================== EDUCATION ==================== -->
<div class="section">
<h2>🎓 Education</h2>

<div class="edu-item">
  <span class="edu-year">2024 – Present</span>
  <div class="edu-detail">
    <h4>Ph.D. in Computer Science and Technology</h4>
    <p>Sun Yat-sen University (SYSU), Guangzhou, China</p>
    <p>Advisor: Prof. Yanghui Rao</p>
  </div>
</div>

<div class="edu-item">
  <span class="edu-year">2020 – 2023</span>
  <div class="edu-detail">
    <h4>M.Eng. in Computer Science and Technology</h4>
    <p>North China Electric Power University (NCEPU), Beijing, China</p>
  </div>
</div>

<div class="edu-item">
  <span class="edu-year">2016 – 2020</span>
  <div class="edu-detail">
    <h4>B.Eng. in Computer Science and Technology</h4>
    <p>North China Electric Power University (NCEPU), Beijing, China</p>
  </div>
</div>

</div>

<!-- ==================== EXPERIENCE ==================== -->
<div class="section">
<h2>💼 Experience</h2>

<div class="exp-item">
  <span class="exp-year">2023 – Present</span>
  <div class="exp-detail">
    <h4>Research Intern — <a href="https://www.zhipuai.cn/" target="_blank">Zhipu AI</a></h4>
    <p>Working on large language models and data mining applications, including academic knowledge graph construction and anomaly detection.</p>
  </div>
</div>

</div>

<!-- ==================== SERVICES ==================== -->
<div class="section">
<h2>🤝 Academic Services</h2>

<p>Reviewer for top-tier AI/NLP conferences and journals. <em>(Details to be updated)</em></p>

</div>

<!-- ==================== CONTACT ==================== -->
<div class="section">
<div class="contact-section">
  <h2 style="border:none; text-align:center;">📬 Contact</h2>
  <p>
    Feel free to reach out for collaboration or discussion!<br>
    📧 <a href="mailto:pangyh8@mail2.sysu.edu.cn">pangyh8@mail2.sysu.edu.cn</a>
    &nbsp;|&nbsp;
    💻 <a href="https://github.com/pangaass" target="_blank">GitHub</a>
    &nbsp;|&nbsp;
    🎓 <a href="https://scholar.google.com/citations?user=doF4h50AAAAJ&hl=zh-CN&oi=ao" target="_blank">Google Scholar</a>
  </p>
</div>
</div>

<div style="text-align:center; color:#aaa; font-size:0.8em; margin-top:40px;">
  Last updated: Feb 2026 &nbsp;|&nbsp; Powered by <a href="https://pages.github.com/" style="color:#aaa;">GitHub Pages</a>
</div>
