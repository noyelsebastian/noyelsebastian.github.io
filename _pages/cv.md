---
layout: archive
title: "Curriculum Vitae <a href='/files/NOYEL_CV.pdf' download><i class='fas fa-file-pdf' style='color: #d9534f; font-size: 0.8em; margin-left: 10px;'></i></a>"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/leaflet.css" />
<script src="https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/leaflet.js"></script>

<style>

/* ===== GLOBAL ===== */
.section {
  margin-top: 35px;
}

.section-title {
  font-size: 1.4em;
  font-weight: 600;
  border-bottom: 2px solid #eee;
  padding-bottom: 6px;
  margin-bottom: 15px;
}

/* ===== ENTRY LAYOUT ===== */
.entry {
  display: flex;
  justify-content: space-between;
  margin-bottom: 18px;
}

.entry-left {
  max-width: 75%;
}

.entry-right {
  text-align: right;
  color: #777;
  font-size: 0.9em;
  white-space: nowrap;
}

/* ===== TEXT STYLES ===== */
.title {
  font-weight: 600;
  font-size: 1.05em;
}

.subtitle {
  color: #444;
  font-size: 0.95em;
}

.details {
  font-size: 0.9em;
  color: #555;
  margin-top: 3px;
}

/* ===== HIGHLIGHT CURRENT ===== */
.current .title {
  font-weight: 700;
}

/* ===== MAP BUTTON ===== */
.map-button {
  background-color: #001f3f;
  color: white;
  border: none;
  border-radius: 4px;
  padding: 6px 12px;
  font-size: 0.8em;
  cursor: pointer;
  margin-right: 6px;
}

.map-button:hover {
  background-color: #001f3f;
}

/* ===== LIST COMPACT ===== */
.compact-list li {
  margin-bottom: 4px;
}

</style>

---

## General Information

- **Full Name:** Noyel Sebastian  
- **Position:** Senior Research Fellow  
- **Affiliation:** CSWE (CITD), Jawaharlal Nehru University, New Delhi  
- **Email:** noyelaniyara@gmail.com  

---

<div class="section">
<div class="section-title">Education</div>

<div class="entry current">
  <div class="entry-left">
    <div class="title">Ph.D. in Economics</div>
    <div class="subtitle"><strong>CSWE (CITD), Jawaharlal Nehru University, New Delhi</strong></div>
    <div class="details">Advisor: Dr. Rashmi Barua</div>
    <div class="details">Fields: Development Economics (Labor, Health, Gender)</div>
  </div>
  <div class="entry-right">Feb 2023 – Dec 2026 (expected)</div>
</div>

<div class="entry">
  <div class="entry-left">
    <div class="title">Master of Arts in Economics</div>
    <div class="subtitle">University of Kerala, Thiruvananthapuram</div>
    <div class="details">CGPA: 8.50 (Third Rank)</div>
  </div>
  <div class="entry-right">2019 – 2021</div>
</div>

<div class="entry">
  <div class="entry-left">
    <div class="title">Bachelor of Arts in Economics</div>
    <div class="subtitle">Loyola College, Chennai</div>
    <div class="details">CGPA: 8.52</div>
  </div>
  <div class="entry-right">2016 – 2019</div>
</div>

</div>

---

<div class="section">
<div class="section-title">Experience</div>

<div class="entry">
  <div class="entry-left">
    <div class="title">Teaching Assistant</div>
    <div class="subtitle">CSWE, Jawaharlal Nehru University, New Delhi</div>
    <div class="details">Microeconomics I (Graduate Level), Monsoon 2025 (with Prof. Sushama Murty)</div>
    <div class="details">Microeconomics I (Graduate Level), Monsoon 2024 (with Prof. Sushama Murty)</div>
  </div>
  <div class="entry-right">2024 – 2025</div>
</div>

<div class="entry">
  <div class="entry-left">
    <div class="title">Intern</div>
    <div class="subtitle">Rubber Research Institute of India, Ministry of Commerce</div>
  </div>
  <div class="entry-right">2018</div>
</div>

</div>

---

<div class="section">
<div class="section-title">Honors and Awards</div>

<ul class="compact-list">
  <li><strong>2025</strong> — Best Paper Award, MIDS Doctoral Colloquium</li>
  <li><strong>2023</strong> — Best Youth Paper Award, IASSH Conference</li>
  <li><strong>2023</strong> — Best Presentation Award, DG Vaishnav College</li>
  <li><strong>2022</strong> — UGC Junior Research Fellowship (JRF)</li>
  <li><strong>2017</strong> — Loyola Research Park Fellowship</li>
</ul>

</div>

---

<div class="section">
<div class="section-title">Conferences and Presentations</div>

<div id="conference-map" style="height: 450px; width: 100%; border-radius: 8px; border: 1px solid #ddd; margin-bottom: 10px;"></div>

<div style="margin-bottom: 25px;">
  <button onclick="zoomTo([22.9734, 78.6569], 4)" class="map-button">India</button>
  <button onclick="zoomTo([20, 0], 2)" class="map-button">International</button>
</div>

</div>

{% raw %}
<script>
document.addEventListener("DOMContentLoaded", function () {

  var map = L.map('conference-map').setView([22.9734, 78.6569], 4);

  L.tileLayer('https://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}{r}.png', {
    attribution: '&copy; OpenStreetMap &copy; CARTO'
  }).addTo(map);

  var conferences = [
    [26.5123, 80.2329, "<b>IIT Kanpur</b><br>Research Scholar's Day (Mar 2025)"],
    [23.0225, 72.5714, "<b>Ahmedabad University</b><br>Annual Economics Conference (Jan 2026)"],
    [28.5843, 77.2500, "<b>Delhi</b><br>DSE & JNU Conferences"],
    [8.5241, 76.9366, "<b>Thiruvananthapuram</b><br>CDS & Kerala University"],
    [51.5115, -0.1160, "<b>King's College London</b><br>YSI-AHE Conference"],
  ];

  conferences.forEach(function(conf) {
    L.marker([conf[0], conf[1]]).addTo(map).bindPopup(conf[2]);
  });

  function zoomTo(coords, zoomLevel) {
    map.flyTo(coords, zoomLevel, { duration: 1.5 });
  }

  window.zoomTo = zoomTo;

});
</script>
{% endraw %}

---

<div class="section">
<div class="section-title">Skills</div>

<ul class="compact-list">
  <li><strong>Software:</strong> STATA, Python, LaTeX, QGIS</li>
  <li><strong>Languages:</strong> English, Malayalam, Tamil, Hindi, French (Elementary)</li>
</ul>

</div>

---

<div class="section">
<div class="section-title">Other Interests</div>

<ul class="compact-list">
  <li>Quizzing</li>
  <li>Reading (Non-fiction)</li>
  <li>Cooking</li>
</ul>

</div>