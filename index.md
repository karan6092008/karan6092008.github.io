---
layout: home
title: TechReview Zero Hub
---

<style>
/* 1. Global Dark Theme Framework */
:root {
  --bg-color: #0d1117;
  --text-color: #c9d1d9;
  --accent-color: #58a6ff;
  --card-bg: #161b22;
  --table-border: #30363d;
}

.animated-content {
  background-color: var(--bg-color);
  color: var(--text-color);
  padding: 25px;
  border-radius: 8px;
  animation: fadeInUp 0.8s ease-out forwards;
}

@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(15px); }
  to { opacity: 1; transform: translateY(0); }
}

/* 2. Custom Sleek Dark Tables */
.tech-table {
  width: 100%;
  border-collapse: collapse;
  margin: 15px 0 25px 0;
  background-color: var(--card-bg);
}

.tech-table th, .tech-table td {
  border: 1px solid var(--table-border) !important;
  padding: 12px !important;
  text-align: left;
}

.tech-table th {
  background-color: #21262d !important;
  color: var(--accent-color) !important;
}

/* 3. Performance Metric Loading Bars */
.bar-container {
  background-color: #30363d;
  border-radius: 4px;
  width: 100%;
  margin: 4px 0;
}

.bar {
  height: 20px;
  border-radius: 4px;
  background: linear-gradient(90deg, #1f6feb, var(--accent-color));
  width: var(--final-width);
  color: white;
  font-size: 11px;
  font-weight: bold;
  padding-left: 8px;
  display: flex;
  align-items: center;
}
</style>

<div class="animated-content">

<h2>📊 Live Hardware Benchmarks</h2>

<table class="tech-table">
  <thead>
    <tr>
      <th>Processor Engine</th>
      <th>Cinebench R23 Score & Visual Performance Gap</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Intel Core Ultra 7</strong></td>
      <td><div class="bar-container"><div class="bar" style="--final-width: 100%;">16,200 (100%)</div></div></td>
    </tr>
    <tr>
      <td><strong>AMD Ryzen 7</strong></td>
      <td><div class="bar-container"><div class="bar" style="--final-width: 87%; background: linear-gradient(90deg, #d83b01, #ff8c00);">14,100 (87%)</div></div></td>
    </tr>
  </tbody>
</table>

<h2>🎮 Graphics Engine Frame Rates (1440p)</h2>

<table class="tech-table">
  <thead>
    <tr>
      <th>Graphics Card</th>
      <th>Average Performance Metrics</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>NVIDIA RTX 5060</strong></td>
      <td><div class="bar-container"><div class="bar" style="--final-width: 100%; background: linear-gradient(90deg, #107c10, #76b900);">95 FPS (100%)</div></div></td>
    </tr>
    <tr>
      <td><strong>AMD RX 7600 XT</strong></td>
      <td><div class="bar-container"><div class="bar" style="--final-width: 78%; background: linear-gradient(90deg, #d83b01, #e61c24);">74 FPS (78%)</div></div></td>
    </tr>
  </tbody>
</table>

</div>

---

## Dedicated Hardware Reviews
