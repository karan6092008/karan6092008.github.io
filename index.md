---
layout: home
title: TechReview Zero Hub
---

<style>
/* 1. Global Dark Theme Rules */
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

/* 2. Interactive Navigation Tabs */
.tab-container {
  display: flex;
  gap: 10px;
  margin: 20px 0;
  border-bottom: 2px solid var(--table-border);
  padding-bottom: 10px;
}

.tab-btn {
  background: #21262d;
  color: var(--text-color);
  border: 1px solid var(--table-border);
  padding: 8px 16px;
  border-radius: 20px;
  cursor: pointer;
  font-weight: bold;
  transition: all 0.3s ease;
}

.tab-btn:hover {
  border-color: var(--accent-color);
}

.tab-btn.active {
  background: var(--accent-color);
  color: #ffffff;
  border-color: var(--accent-color);
}

/* 3. Hide/Show Content Classes */
.filter-item {
  display: block;
  animation: fadeIn 0.4s ease-in-out;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* 4. Custom Table & Progress Bar styles */
table { width: 100%; border-collapse: collapse; margin-top: 15px; background-color: var(--card-bg); }
th, td { border: 1px solid var(--table-border) !important; padding: 12px !important; }
th { background-color: #21262d !important; color: var(--accent-color) !important; }
.bar-container { background-color: #30363d; border-radius: 4px; width: 100%; margin: 4px 0; }
.bar { height: 20px; border-radius: 4px; background: linear-gradient(90deg, #1f6feb, var(--accent-color)); width: var(--final-width); color: white; font-size: 11px; font-weight: bold; padding-left: 8px; display: flex; align-items: center; }
</style>

<div class="animated-content">

<!-- Category Navigation Interface -->
<div class="tab-container">
  <button class="tab-btn active" onclick="filterCategory('all')">All Tech</button>
  <button class="tab-btn" onclick="filterCategory('cpu')">CPUs</button>
  <button class="tab-btn" onclick="filterCategory('gpu')">GPUs</button>
  <button class="tab-btn" onclick="filterCategory('laptop')">Laptops</button>
</div>

<!-- DATA SECTION: CPUs -->
<div class="filter-item item-cpu">
### 📊 Processor Metrics (Cinebench R23)
| Hardware Engine | Cinebench R23 Score & Visual Gap |
| :--- | :--- |
| **Intel Core Ultra 7** | <div class="bar-container"><div class="bar" style="--final-width: 100%;">16,200 (100%)</div></div> |
| **AMD Ryzen 7** | <div class="bar-container"><div class="bar" style="--final-width: 87%; background: linear-gradient(90deg, #d83b01, #ff8c00);">14,100 (87%)</div></div> |
</div>

<!-- DATA SECTION: GPUs -->
<div class="filter-item item-gpu">
### 🎮 Graphics Performance (Time Spy FPS)
| Card Engine | Average 1440p Frame Metrics |
| :--- | :--- |
| **NVIDIA RTX 5060** | <div class="bar-container"><div class="bar" style="--final-width: 100%; background: linear-gradient(90deg, #107c10, #76b900);">95 FPS (100%)</div></div> |
| **AMD RX 7600 XT** | <div class="bar-container"><div class="bar" style="--final-width: 78%; background: linear-gradient(90deg, #d83b01, #e61c24);">74 FPS (78%)</div></div> |
</div>

<!-- DATA SECTION: Laptops -->
<div class="filter-item item-laptop">
### 💻 Laptop Spec Roundups
| Feature | Premium Laptop A | Budget Competitor B |
| :--- | :--- | :--- |
| **Processor** | Intel Core Ultra 7 | AMD Ryzen 7 |
| **Battery Life** | ~9 Hours | ~12 Hours |
</div>

</div>

<!-- JavaScript Engine to Filter Content Dynamically -->
<script>
function filterCategory(category) {
  // Update active button state
  const buttons = document.querySelectorAll('.tab-btn');
  buttons.forEach(btn => btn.classList.remove('active'));
  event.target.classList.add('active');

  // Filter content blocks
  const items = document.querySelectorAll('.filter-item');
  items.forEach(item => {
    if (category === 'all') {
      item.style.display = 'block';
    } else if (item.classList.contains('item-' + category)) {
      item.style.display = 'block';
    } else {
      item.style.display = 'none';
    }
  });
}
  <style>
/* Responsive Advertisement / Affiliate Grid Layout */
.main-layout {
  display: grid;
  grid-template-columns: 3fr 1fr;
  gap: 20px;
}
.ad-sidebar {
  background: #161b22;
  border: 1px solid #30363d;
  padding: 15px;
  border-radius: 8px;
  height: max-content;
}
.banner-space {
  background: #21262d;
  border: 2px dashed #58a6ff;
  color: #8b949e;
  padding: 40px 10px;
  text-align: center;
  border-radius: 4px;
  font-size: 12px;
  margin-bottom: 15px;
}
@media (max-width: 768px) {
  .main-layout { grid-template-columns: 1fr; }
}
</style>

<div class="main-layout">

  <div class="content-side">
    </div>

  <div class="ad-sidebar">
    <h3>📢 Deals of the Week</h3>
    
    <div class="banner-space">
      <strong>[AD PLACEHOLDER]</strong><br>
      <a href="YOUR_AFFILIATE_LINK" style="color:#58a6ff;">RTX 4070 Laptop Deal 15% OFF</a>
    </div>

    <div class="banner-space">
      <strong>[SPONSOR ZONE]</strong><br>
      Contact us to feature your tech hardware here.
    </div>
  </div>

</div>
</script>
