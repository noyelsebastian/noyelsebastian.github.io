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
  background-color: #003366;
}
</style>


## General Information

- **Full Name:** Noyel Sebastian  
- **Position:** Senior Research Fellow  
- **Affiliation:** CSWE (CITD), Jawaharlal Nehru University, New Delhi  
- **Email:** noyelaniyara@gmail.com  
- **Date of Birth:** 16 February 1998  

---

## Education

**Ph.D. in Economics**  
CSWE (CITD), Jawaharlal Nehru University, New Delhi  
*February 2023 – February 2027 (expected)*  
- Advisor: <a href="https://sites.google.com/site/rbaruabhowmik/">Dr. Rashmi Barua</a>  
- Research Areas: Development Economics, Labour Economics, Health Economics  

**Master of Arts in Economics**  
Department of Economics, University of Kerala, Thiruvananthapuram  
*2019 – 2021*  
- CGPA: 8.50 (Third Rank)

**Bachelor of Arts in Economics**  
Loyola College, Chennai, Tamil Nadu  
*2016 – 2019*  
- CGPA: 8.52

---

## Experience

**Teaching Assistant**  
CSWE, Jawaharlal Nehru University, New Delhi  
*2024 – 2025*  
- Microeconomics I (Graduate Level), Monsoon 2025  
  (with <a href="https://www.jnu.ac.in/content/sushama">Prof. Sushama Murty</a>)  
- Microeconomics I (Graduate Level), Monsoon 2024  
  (with <a href="https://www.jnu.ac.in/content/sushama">Prof. Sushama Murty</a>)  

**Intern**  
Economic Research Wing, Rubber Research Institute of India  
Ministry of Commerce and Industry, Government of India  
*2018*

---

## Honors and Awards

- **2025** — Best Paper Award, 3rd MIDS Doctoral Colloquium  
- **2023** — Best Youth Paper Award, IASSH International Conference  
- **2023** — Best Presentation Award, International Conference, DG Vaishnav College, Chennai  
- **2022** — University Grants Commission – Junior Research Fellowship (UGC-JRF)  
- **2017** — Loyola Research Park Fellowship  

---

## Conferences and Research Presentations

<div id="conference-map" style="height: 450px; width: 100%; border-radius: 8px; border: 1px solid #ddd; margin-bottom: 10px;"></div>

<div style="margin-bottom: 30px;">
  <button onclick="zoomTo([22.9734, 78.6569], 4)" class="map-button">
    Focus: India
  </button>

  <button onclick="zoomTo([20, 0], 2)" class="map-button">
    Focus: World
  </button>
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
    [28.5843, 77.2500, "<b>Delhi School of Economics</b><br>&bull; Young Scholar’s Conference (Feb 2025)"],
    [8.5241, 76.9366, "<b>CDS Thiruvananthapuram</b><br>&bull; Doctoral Colloquium (Mar 2025)"],
    [30.6425, 76.7179, "<b>Plaksha University, Chandigarh</b><br>&bull; LEO Economics Conference (Apr 2025)"],
    [34.0837, 74.7973, "<b>University of Kashmir</b><br>&bull; Annual CECFEE Research & Policy Workshop (Nov 2025)"],
    [13.0064, 80.2548, "<b>MIDS, Chennai</b><br>&bull; 3rd MIDS Doctoral Colloquium (Oct 2025)"],
    [28.5398, 77.5390, "<b>Sharda University, Greater Noida</b><br>&bull; IASSH 18th International Conference (2023)"],
    [-15.7938, -47.8828, "<b>Brasilia, Brazil</b><br>&bull; 6th Meeting of the Society of Family and Gender Economics (2025)"],
    [51.5115, -0.1160, "<b>King's College London</b><br>&bull; 27th AHE Conference (June 2025, Online)"],
    [8.5074, 76.9511, "<b>University of Kerala</b><br>&bull; CMASE 3.0 (2022)"],
    [28.5397, 77.1661, "<b>Jawaharlal Nehru University (JNU)</b><br>&bull; Sukhamoy Chakravarty Chair - Young Scholars Conference, CESP (Oct 2025)"],
    [22.5763, 88.3639, "<b>IIM Calcutta</b><br>&bull; Amitava Bose Memorial Workshop (July 2025)"],
    [13.0827, 80.2707, "<b>DG Vaishnav College, Chennai</b><br>&bull; International Conference (2023)"]
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


**2026**
- 7th Annual Economics Conference, Ahmedabad University  

**2025**
- Young Scholar’s Conference, Delhi School of Economics  
- Research Scholar’s Day, IIT Kanpur  
- Doctoral Colloquium, CDS Thiruvananthapuram  
- LEO Economics Conference, Plaksha University, Chandigarh  
- 27th AHE Conference — YSI Editorial Session, King’s College London *(online)*  
- Amitava Bose Memorial Annual Workshop, IIM Calcutta  
- 6th Meeting of the Society of Family and Gender Economics, Brasília, Brazil *(accepted; could not attend)*  
- 3rd MIDS Doctoral Colloquium, Adyar, Chennai  
- Sukhamoy Chakravarty Chair – Young Scholars Conference, CESP, JNU  
- Annual CECFEE Research & Policy Workshop, University of Kashmir  

**2023**
- IASSH 18th International Conference, Sharda University, Greater Noida  
- International Conference, DG Vaishnav College, Chennai  

**2022**
- CMASE 3.0, University of Kerala  

---

## Skills and Expertise

**Computer & Software**
- STATA, Python, LaTeX, QGIS  

**Courses**
- <a href="https://drive.google.com/file/d/1BMOptktD4c_nPMpwIl6r0U5qLB39pkl5/view">
  Designing and Running Randomized Evaluations (MITx | JPAL102x)</a>  
- <a href="https://drive.google.com/file/d/12H7xbpCov6FZAUPt2TA9UuVE91_b3tlk/view">
  IZA / FCDO Online Development Economics Course</a>  

**Languages**
- English, Malayalam, Tamil, Hindi  
- French (Elementary Proficiency)

---

## Other Interests

- Quizzing  
- Reading (Non-fiction)  
- Cooking  
