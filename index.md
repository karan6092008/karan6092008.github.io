---
layout: home
title: TechReview Zero Hub
---

<style>
/* 1. Global Dark Mode & Animation Variables */
:root {
  --bg-color: #0d1117;
  --text-color: #c9d1d9;
  --accent-color: #58a6ff;
  --card-bg: #161b22;
  --table-border: #30363d;
}

/* Apply Dark Mode directly into the page hub container */
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

/* 2. Sleek Dark Mode Table Styling */
table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 15px;
  background-color: var(--card-bg);
}

th, td {
  border: 1px solid var(--table-border) !important;
  padding: 12px !important;
}

th {
  background-color: #21262d !important;
  color: var(--accent-color) !important;
}

tr:hover {
  background-color: #21262d !important;
  transform: scale(1.005);
  transition: all 0.2s ease;
}

/* 3. Pure CSS Visual Benchmark Bars Animation */
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
  width: 0; /* Starts at 0 for animation */
  animation: loadBar 1.2s cubic-bezier(0.1, 0.8, 0.3, 1) forwards;
  animation-delay: 0.4s;
  color: white;
  font-size: 11px;
  font-weight: bold;
  padding-left: 8px;
  display: flex;
  align-items: center;
}

@keyframes loadBar {
  to { width: var(--final-width); }
}
</style>

<div class="animated-content">

## 📊 Live Frame-Rate & Benchmark Metrics

Below is a breakdown of rendering performance across the latest silicon chips. Notice the comparative multi-core rendering load lines:

| Hardware Engine | Cinebench R23 Score & Visual Gap |
| :--- | :--- |
| **Intel Core Ultra 7** | <div class="bar-container"><div class="bar" style="--final-width: 100%;">16,200 (100%)</div></div> |
| **AMD Ryzen 7** | <div class="bar-container"><div class="bar" style="--final-width: 87%; background: linear-gradient(90deg, #d83b01, #ff8c00);">14,100 (87%)</div></div> |
| **Apple M3 Pro** | <div class="bar-container"><div class="bar" style="--final-width: 93%; background: linear-gradient(90deg, #8e44ad, #a3e4d7);">15,120 (93%)</div></div> |

---

## 💻 Latest Hardware Comparisons

| Feature | Premium Laptop A | Budget Competitor B |
| :--- | :--- | :--- |
| **Processor** | Intel Core Ultra 7 | AMD Ryzen 7 |
| **Graphics** | RTX 4060 Mobile | Radeon 780M (Integrated) |
| **Battery Life** | ~9 Hours | ~12 Hours |

</div>
