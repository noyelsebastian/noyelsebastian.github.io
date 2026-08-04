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
    <div class="details">Advisor: <a href="https://sites.google.com/site/rbaruabhowmik/">Dr. Rashmi Barua</a> </div>
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
    <div class="details">Microeconomics I (Graduate Level), Monsoon 2025 (with <a href="https://www.jnu.ac.in/content/sushama">Prof. Sushama Murty</a>)</div>
    <div class="details">Microeconomics I (Graduate Level), Monsoon 2024 (with <a href="https://www.jnu.ac.in/content/sushama">Prof. Sushama Murty</a>)</div>
  </div>
  <div class="entry-right">2024 – 2025</div>
</div>

<div class="entry">
  <div class="entry-left">
    <div class="title">Intern</div>
    <div class="subtitle">Economic Research Wing, Rubber Research Institute of India, Government of India</div>
  </div>
  <div class="entry-right">2018</div>
</div>

</div>

---

<div class="section">
<div class="section-title">Honors and Awards</div>

<ul class="compact-list">
  <li><strong>2025</strong> — Best Paper Award, 3rd MIDS Doctoral Colloquium</li>
  <li><strong>2023</strong> — Best Youth Paper Award, IASSH International Conference</li>
  <li><strong>2023</strong> — Best Presentation Award,International Conference, DG Vaishnav College</li>
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
    [26.5123, 80.2329, "<b>IIT Kanpur</b><br>&bull; Research Scholar's Day (Mar 2025)"],
    [23.0225, 72.5714, "<b>Ahmedabad University</b><br>&bull; 7th Annual Economics Conference (Jan 2026)"],
    [28.5843, 77.2500, "<b>Delhi</b><br>&bull; Young Scholar’s Conference, Delhi School of Economics (Feb 2025)<br>&bull; Sukhamoy Chakravarty Chair - Young Scholars Conference, JNU (Oct 2025)<br>&bull; CDE–IEDS International Conference, Delhi School of Economics (June 2026), "],
    [8.5241, 76.9366, "<b>Thiruvananthapuram</b><br>&bull; CDS Doctoral Colloquium (Mar 2025)<br>&bull; CMASE 3.0, University of Kerala (2022)"],
    [30.6425, 76.7179, "<b>Plaksha University, Chandigarh</b><br>&bull; LEO Economics Conference (Apr 2025)"],
    [34.0837, 74.7973, "<b>University of Kashmir</b><br>&bull; Annual CECFEE Research & Policy Workshop (Nov 2025)"],
    [28.5398, 77.5390, "<b>Sharda University, Greater Noida</b><br>&bull; IASSH 18th International Conference (2023)"],
    [-15.7938, -47.8828, "<b>Brasilia, Brazil</b><br>&bull; 6th Meeting of the Society of Family and Gender Economics (2025, accepted; could not attend)"],
    [51.5115, -0.1160, "<b>King's College London</b><br>&bull; 27th YSI-AHE Conference (June 2025, Online)"],
    [40.2033, -8.4103, "<b>Coimbra, Portugal</b><br>&bull; Annual Heterodox Economics Conference, University of Coimbra (2026, accepted; could not attend)"],
    [22.5763, 88.3639, "<b>IIM Calcutta</b><br>&bull; Amitava Bose Memorial Workshop (July 2025)"],
    [13.0827, 80.2707, "<b>Chennai</b><br>&bull; MIDS Doctoral Colloquium (Oct 2025)<br>&bull; DG Vaishnav College Conference (2023)"],
  ];

  conferences.forEach(function(conf) {
    L.marker([conf[0], conf[1]]).addTo(map).bindPopup(conf[2]);
  });

  function zoomTo(coords, zoomLevel) {
    map.flyTo(coords, zoomLevel, { duration: 1.5 });
  }

  window.zoomTo = zoomTo;

  setTimeout(function () {
    map.invalidateSize();
  }, 200);

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
<div class="section-title">Professional Training</div>

<ul class="compact-list">
  <li>
    <strong>MITx / J-PAL102x</strong> —
    <a href="https://drive.google.com/file/d/1BMOptktD4c_nPMpwIl6r0U5qLB39pkl5/view" target="_blank">
      Designing and Running Randomized Evaluations
    </a>
  </li>

  <li>
    <strong>IZA–FCDO</strong> —
    <a href="https://drive.google.com/file/d/12H7xbpCov6FZAUPt2TA9UuVE91_b3tlk/view" target="_blank">
      Development Economics Course
    </a>
  </li>
</ul>

</div>
