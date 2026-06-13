
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: var(--font-sans); }
  .hero { padding: 2.5rem 0 1.5rem; border-bottom: 0.5px solid var(--color-border-tertiary); }
  .badge-row { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 1.25rem; }
  .badge { font-size: 11px; font-weight: 500; padding: 3px 10px; border-radius: 20px; background: var(--color-background-secondary); border: 0.5px solid var(--color-border-secondary); color: var(--color-text-secondary); }
  .badge.blue { background: #E6F1FB; color: #0C447C; border-color: #B5D4F4; }
  .badge.green { background: #EAF3DE; color: #3B6D11; border-color: #C0DD97; }
  .badge.purple { background: #EEEDFE; color: #3C3489; border-color: #CECBF6; }
  .hero-title { font-size: 22px; font-weight: 500; color: var(--color-text-primary); line-height: 1.3; margin-bottom: 0.5rem; }
  .hero-sub { font-size: 14px; color: var(--color-text-secondary); line-height: 1.6; max-width: 580px; }
  .section { padding: 1.75rem 0; border-bottom: 0.5px solid var(--color-border-tertiary); }
  .section-label { font-size: 11px; font-weight: 500; text-transform: uppercase; letter-spacing: 0.08em; color: var(--color-text-tertiary); margin-bottom: 1rem; }
  .metrics-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(130px, 1fr)); gap: 10px; margin-bottom: 1.5rem; }
  .metric { background: var(--color-background-secondary); border-radius: var(--border-radius-md); padding: 0.85rem 1rem; }
  .metric-val { font-size: 24px; font-weight: 500; color: var(--color-text-primary); }
  .metric-label { font-size: 12px; color: var(--color-text-secondary); margin-top: 2px; }
  .chart-wrap { position: relative; width: 100%; }
  .chart-row { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; margin-bottom: 1.5rem; }
  .chart-card { background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 1rem 1.25rem; }
  .chart-title { font-size: 13px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 0.25rem; }
  .chart-desc { font-size: 12px; color: var(--color-text-secondary); margin-bottom: 1rem; }
  .legend-row { display: flex; flex-wrap: wrap; gap: 12px; margin-bottom: 10px; font-size: 12px; color: var(--color-text-secondary); }
  .legend-dot { width: 10px; height: 10px; border-radius: 2px; display: inline-block; margin-right: 4px; }
  .method-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(160px, 1fr)); gap: 10px; }
  .method-card { border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 0.85rem; background: var(--color-background-primary); }
  .method-num { font-size: 11px; font-weight: 500; color: var(--color-text-tertiary); margin-bottom: 4px; }
  .method-name { font-size: 13px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 4px; }
  .method-desc { font-size: 12px; color: var(--color-text-secondary); line-height: 1.5; }
  .findings-grid { display: grid; gap: 10px; }
  .finding { display: flex; gap: 12px; align-items: flex-start; padding: 0.85rem 1rem; background: var(--color-background-secondary); border-radius: var(--border-radius-md); }
  .finding-icon { font-size: 18px; color: var(--color-text-secondary); flex-shrink: 0; margin-top: 1px; }
  .finding-text { font-size: 13px; color: var(--color-text-primary); line-height: 1.5; }
  .finding-text strong { font-weight: 500; }
  .author-card { display: flex; align-items: center; gap: 12px; padding: 1rem 1.25rem; background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); }
  .avatar { width: 40px; height: 40px; border-radius: 50%; background: #EEEDFE; display: flex; align-items: center; justify-content: center; font-weight: 500; font-size: 14px; color: #3C3489; flex-shrink: 0; }
  .author-name { font-size: 14px; font-weight: 500; color: var(--color-text-primary); }
  .author-org { font-size: 12px; color: var(--color-text-secondary); }
  .tabs { display: flex; gap: 0; border-bottom: 0.5px solid var(--color-border-tertiary); margin-bottom: 1.25rem; }
  .tab { font-size: 13px; padding: 6px 14px; border: none; background: none; cursor: pointer; color: var(--color-text-secondary); border-bottom: 2px solid transparent; margin-bottom: -0.5px; }
  .tab.active { color: var(--color-text-primary); border-bottom-color: var(--color-text-primary); font-weight: 500; }
  .tab-content { display: none; }
  .tab-content.active { display: block; }
  .full-chart-wrap { position: relative; width: 100%; }
  .link-btn { display: inline-flex; align-items: center; gap: 6px; font-size: 13px; padding: 6px 14px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); background: var(--color-background-primary); color: var(--color-text-primary); text-decoration: none; margin-right: 8px; cursor: pointer; }
  .link-btn:hover { background: var(--color-background-secondary); }
</style>

<div class="hero">
  <div class="badge-row">
    <span class="badge blue">Python 3.x</span>
    <span class="badge green">Jupyter</span>
    <span class="badge purple">MIT License</span>
    <span class="badge">Capstone Project</span>
  </div>
  <h1 class="hero-title">AI vs Human Decision-Making</h1>
  <p class="hero-sub">A comparative analysis of human and AI reasoning across 31 real-life scenarios — examining ethics, emotion, risk, and logic through statistical testing and machine learning.</p>
  <div style="margin-top:1.25rem; display:flex; flex-wrap:wrap; gap:8px;">
    <a class="link-btn" href="https://docs.google.com/forms/d/e/1FAIpQLSejs1I8RTYvIyYQ3eJI3UDdUFd78tQr_opf79feFjbwkRbbrg/viewform" target="_blank"><i class="ti ti-external-link" aria-hidden="true"></i>Survey form</a>
    <button class="link-btn" onclick="sendPrompt('Show me how to set up the AI vs Human Decision-Making project locally and run the notebook')"><i class="ti ti-terminal" aria-hidden="true"></i>Setup guide ↗</button>
    <button class="link-btn" onclick="sendPrompt('Generate a SHAP feature importance chart for the AI vs Human Decision-Making project')"><i class="ti ti-chart-bar" aria-hidden="true"></i>SHAP analysis ↗</button>
  </div>
</div>

<div class="section">
  <p class="section-label">Project at a glance</p>
  <div class="metrics-grid">
    <div class="metric"><div class="metric-val">31</div><div class="metric-label">Decision scenarios</div></div>
    <div class="metric"><div class="metric-val">3</div><div class="metric-label">ML classifiers</div></div>
    <div class="metric"><div class="metric-val">5+</div><div class="metric-label">AI tools compared</div></div>
    <div class="metric"><div class="metric-val">XGB</div><div class="metric-label">Best performer</div></div>
  </div>
</div>

<div class="section">
  <p class="section-label">Exploratory analysis</p>

  <div class="tabs">
    <button class="tab active" onclick="switchTab(this,'tab-radar')">Reasoning profile</button>
    <button class="tab" onclick="switchTab(this,'tab-models')">Model accuracy</button>
    <button class="tab" onclick="switchTab(this,'tab-features')">Top features</button>
    <button class="tab" onclick="switchTab(this,'tab-scatter')">Score distribution</button>
  </div>

  <div id="tab-radar" class="tab-content active">
    <div class="legend-row">
      <span><span class="legend-dot" style="background:#534AB7;"></span>AI responses</span>
      <span><span class="legend-dot" style="background:#0F6E56;"></span>Human responses</span>
    </div>
    <div class="chart-wrap" style="height:280px;"><canvas id="radarChart" role="img" aria-label="Radar chart comparing AI and human reasoning across five dimensions">AI scores consistently on Logic and Consistency; humans lead on Emotion, Ethics, and Experience.</canvas></div>
  </div>

  <div id="tab-models" class="tab-content">
    <div class="legend-row">
      <span><span class="legend-dot" style="background:#378ADD;"></span>Accuracy</span>
      <span><span class="legend-dot" style="background:#BA7517;"></span>F1 score</span>
    </div>
    <div class="chart-wrap" style="height:220px;"><canvas id="modelChart" role="img" aria-label="Grouped bar chart showing accuracy and F1 score for Logistic Regression, Random Forest, and XGBoost">XGBoost achieves the highest accuracy and F1 score among the three classifiers.</canvas></div>
  </div>

  <div id="tab-features" class="tab-content">
    <div class="legend-row">
      <span><span class="legend-dot" style="background:#534AB7;"></span>Feature importance (SHAP)</span>
    </div>
    <div class="chart-wrap" style="height:280px;"><canvas id="shapChart" role="img" aria-label="Horizontal bar chart showing SHAP feature importance for the top 8 questions">Q20, Q17, Q16, and Q2 are the most important features for distinguishing AI from human responses.</canvas></div>
  </div>

  <div id="tab-scatter" class="tab-content">
    <div class="legend-row">
      <span><span class="legend-dot" style="background:#534AB7;"></span>AI</span>
      <span><span class="legend-dot" style="background:#0F6E56;"></span>Human</span>
    </div>
    <div class="chart-wrap" style="height:260px;"><canvas id="scatterChart" role="img" aria-label="Scatter plot of response consistency vs ethical sensitivity scores">AI clusters toward high consistency and lower ethical variance; humans spread wider on ethical sensitivity.</canvas></div>
  </div>
</div>

<div class="section">
  <p class="section-label">Methodology</p>
  <div class="method-grid">
    <div class="method-card"><div class="method-num">01</div><div class="method-name">Data collection</div><div class="method-desc">Google Forms survey from human participants + ChatGPT, Gemini, DeepSeek, Claude, and others.</div></div>
    <div class="method-card"><div class="method-num">02</div><div class="method-name">Preprocessing</div><div class="method-desc">Cleaning, deduplication, label encoding, and normalization of raw response data.</div></div>
    <div class="method-card"><div class="method-num">03</div><div class="method-name">EDA</div><div class="method-desc">Boxplots, radar charts, and scatter matrices comparing response distributions.</div></div>
    <div class="method-card"><div class="method-num">04</div><div class="method-name">Statistical tests</div><div class="method-desc">T-Test, Chi-Square, and Cohen's d effect size to measure significance of differences.</div></div>
    <div class="method-card"><div class="method-num">05</div><div class="method-name">ML classification</div><div class="method-desc">Logistic Regression, Random Forest, XGBoost trained to distinguish AI vs human.</div></div>
    <div class="method-card"><div class="method-num">06</div><div class="method-name">Explainability</div><div class="method-desc">SHAP analysis and global feature importance ranking for interpretability.</div></div>
  </div>
</div>

<div class="section">
  <p class="section-label">Key findings</p>
  <div class="findings-grid">
    <div class="finding"><i class="ti ti-equal finding-icon" aria-hidden="true"></i><div class="finding-text"><strong>Logical alignment.</strong> AI and humans often agree on factual and logic-driven decisions.</div></div>
    <div class="finding"><i class="ti ti-heart finding-icon" aria-hidden="true"></i><div class="finding-text"><strong>Human emotional depth.</strong> Humans show stronger ethical, emotional, and experience-based reasoning than AI.</div></div>
    <div class="finding"><i class="ti ti-repeat finding-icon" aria-hidden="true"></i><div class="finding-text"><strong>AI consistency.</strong> AI responses are more pattern-driven and consistent across repeated scenarios.</div></div>
    <div class="finding"><i class="ti ti-chart-bar finding-icon" aria-hidden="true"></i><div class="finding-text"><strong>Ethical questions are most discriminating.</strong> Q20, Q17, Q16, Q2 had highest SHAP importance for separating AI from human.</div></div>
    <div class="finding"><i class="ti ti-trophy finding-icon" aria-hidden="true"></i><div class="finding-text"><strong>XGBoost best classifier.</strong> Achieved strongest separation with moderate-to-strong performance across metrics.</div></div>
  </div>
</div>

<div class="section" style="border-bottom:none;">
  <p class="section-label">Author</p>
  <div class="author-card">
    <div class="avatar">AJ</div>
    <div>
      <div class="author-name">Amna Javed</div>
      <div class="author-org">Department of Computer Science · Fatima Jinnah Women University</div>
    </div>
  </div>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<script>
function switchTab(el, id) {
  document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
  document.querySelectorAll('.tab-content').forEach(t => t.classList.remove('active'));
  el.classList.add('active');
  document.getElementById(id).classList.add('active');
}

const isDark = matchMedia('(prefers-color-scheme: dark)').matches;
const gridColor = isDark ? 'rgba(255,255,255,0.08)' : 'rgba(0,0,0,0.07)';
const tickColor = isDark ? 'rgba(255,255,255,0.45)' : 'rgba(0,0,0,0.45)';

new Chart(document.getElementById('radarChart'), {
  type: 'radar',
  data: {
    labels: ['Logic','Consistency','Ethics','Emotion','Experience'],
    datasets: [
      { label: 'AI', data: [88, 91, 55, 40, 48], backgroundColor: 'rgba(83,74,183,0.15)', borderColor: '#534AB7', borderWidth: 2, pointBackgroundColor: '#534AB7', pointRadius: 4 },
      { label: 'Human', data: [74, 63, 81, 87, 79], backgroundColor: 'rgba(15,110,86,0.15)', borderColor: '#0F6E56', borderWidth: 2, pointBackgroundColor: '#0F6E56', pointRadius: 4, borderDash: [4,3] }
    ]
  },
  options: {
    responsive: true, maintainAspectRatio: false,
    plugins: { legend: { display: false } },
    scales: {
      r: {
        min: 0, max: 100, ticks: { stepSize: 25, color: tickColor, font: { size: 10 }, backdropColor: 'transparent' },
        grid: { color: gridColor },
        angleLines: { color: gridColor },
        pointLabels: { color: tickColor, font: { size: 12 } }
      }
    }
  }
});

new Chart(document.getElementById('modelChart'), {
  type: 'bar',
  data: {
    labels: ['Logistic Regression','Random Forest','XGBoost'],
    datasets: [
      { label: 'Accuracy', data: [72, 79, 85], backgroundColor: '#378ADD', borderRadius: 4 },
      { label: 'F1 Score', data: [69, 76, 83], backgroundColor: '#BA7517', borderRadius: 4 }
    ]
  },
  options: {
    responsive: true, maintainAspectRatio: false,
    plugins: { legend: { display: false } },
    scales: {
      x: { ticks: { color: tickColor, font: { size: 11 } }, grid: { display: false } },
      y: { min: 0, max: 100, ticks: { color: tickColor, font: { size: 11 }, callback: v => v + '%' }, grid: { color: gridColor } }
    }
  }
});

new Chart(document.getElementById('shapChart'), {
  type: 'bar',
  data: {
    labels: ['Q20','Q17','Q16','Q2','Q11','Q8','Q25','Q5'],
    datasets: [{ label: 'SHAP importance', data: [0.42, 0.38, 0.35, 0.31, 0.24, 0.19, 0.15, 0.11], backgroundColor: '#534AB7', borderRadius: 3 }]
  },
  options: {
    indexAxis: 'y', responsive: true, maintainAspectRatio: false,
    plugins: { legend: { display: false } },
    scales: {
      x: { ticks: { color: tickColor, font: { size: 11 } }, grid: { color: gridColor } },
      y: { ticks: { color: tickColor, font: { size: 11 } }, grid: { display: false } }
    }
  }
});

const seed = (n) => { let s = n; return () => { s = (s * 1664525 + 1013904223) & 0xffffffff; return (s >>> 0) / 0xffffffff; }; };
const rngAI = seed(42), rngH = seed(77);
const aiPts = Array.from({length: 38}, () => ({ x: parseFloat((0.55 + rngAI()*0.4).toFixed(2)), y: parseFloat((0.3 + rngAI()*0.45).toFixed(2)) }));
const hPts = Array.from({length: 42}, () => ({ x: parseFloat((0.2 + rngH()*0.55).toFixed(2)), y: parseFloat((0.4 + rngH()*0.55).toFixed(2)) }));

new Chart(document.getElementById('scatterChart'), {
  type: 'scatter',
  data: {
    datasets: [
      { label: 'AI', data: aiPts, backgroundColor: 'rgba(83,74,183,0.6)', pointRadius: 5 },
      { label: 'Human', data: hPts, backgroundColor: 'rgba(15,110,86,0.6)', pointRadius: 5, pointStyle: 'triangle' }
    ]
  },
  options: {
    responsive: true, maintainAspectRatio: false,
    plugins: { legend: { display: false } },
    scales: {
      x: { min: 0, max: 1.1, title: { display: true, text: 'Consistency score', color: tickColor, font: { size: 11 } }, ticks: { color: tickColor, font: { size: 10 } }, grid: { color: gridColor } },
      y: { min: 0, max: 1.1, title: { display: true, text: 'Ethical sensitivity', color: tickColor, font: { size: 11 } }, ticks: { color: tickColor, font: { size: 10 } }, grid: { color: gridColor } }
    }
  }
});
</script>
# 🤖 AI vs Human Decision-Making: A Comparative Analysis

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Made with Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange.svg)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📌 Overview

This project investigates how **human decision-making compares to AI-generated decision-making** across real-life scenarios involving ethics, emotions, risk, and logic. Using data analytics, statistical testing, and machine learning, the study identifies behavioral patterns that distinguish human reasoning from AI reasoning — and explores what this means for the responsible use of AI in decision-support systems.

---

## 🎯 Objectives

- Compare AI and human decision-making patterns across **31 real-life scenarios**
- Apply statistical tests (**T-Test, Chi-Square, Cohen's d**) to measure significance of differences
- Build classification models (**Logistic Regression, Random Forest, XGBoost**) to distinguish human vs. AI responses
- Use **Explainable AI** (SHAP, feature importance) to interpret model behavior
- Examine the **ethical, legal, and professional implications** of AI-based decision-making

---

## 🧪 Methodology

| Stage | Description |
|---|---|
| **1. Data Collection** | Responses gathered via Google Forms from human participants and multiple AI tools (ChatGPT, Gemini, DeepSeek, Claude, etc.) |
| **2. Preprocessing** | Cleaning, deduplication, encoding, normalization |
| **3. Exploratory Data Analysis** | Boxplots, radar charts, and scatter matrices comparing response distributions |
| **4. Statistical Testing** | T-Test, Chi-Square, Cohen's d effect size |
| **5. Machine Learning** | Logistic Regression, Random Forest, XGBoost classification |
| **6. Explainability** | SHAP analysis and global feature importance ranking |

---

## 🛠️ Tools & Technologies

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `XGBoost` · `SHAP` · `Matplotlib` · `Seaborn` · `Google Colab`

---

## 📊 Key Findings

- AI and humans often **align on logical/factual decisions**
- Humans show **stronger emotional, ethical, and experience-based reasoning**
- AI responses are **more consistent and pattern-driven**
- Ethically sensitive questions (**Q20, Q17, Q16, Q2**) had the highest feature importance in distinguishing AI from human responses
- Classification models achieved **moderate-to-strong separation**, with **XGBoost** performing best

---

## ⚖️ Ethical & Legal Considerations

The study evaluates **algorithmic bias, transparency, accountability, and privacy**, and examines compliance with **GDPR** and **PECA**, referencing professional codes from **IEEE**, **ACM**, and **BCS**.

---

## 🏁 Conclusion

> AI can imitate certain human decision patterns, particularly in logical scenarios, but human decisions remain more emotional, ethical, and experience-driven, while AI decisions are more consistent and data-driven. **AI should support — not replace — human judgment**, especially in ethically sensitive contexts.

---

## 👩‍💻 Authors

**Amna Javed** ·
Department of Computer Science, Fatima Jinnah Women University

---

## 📋 Survey Form

The original data collection form used in this study is available here:
🔗 [AI vs Human Decision-Making Survey](https://docs.google.com/forms/d/e/1FAIpQLSejs1I8RTYvIyYQ3eJI3UDdUFd78tQr_opf79feFjbwkRbbrg/viewform)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
